<p align="center">
  <a href="https://github.com/trimstray/test-your-sysadmin-skills">
    <img src="https://github.com/trimstray/test-your-sysadmin-skills/blob/master/static/img/sysadmin_preview.png" alt="Master">
  </a>
</p>

<br>

<p align="center">"<i>A great Admin doesn't need to know everything, but they should be able to come up with amazing solutions to impossible projects.</i>" - cwheeler33 (ServerFault)</p>

<p align="center">"<i>My skills are making things work, not knowing a billion facts. [...] If I need to fix a system I’ll identify the problem, check the logs and look up the errors. If I need to implement a solution I’ll research the right solution, implement and document it, the later on only really have a general idea of how it works unless I interact with it frequently... it’s why it’s documented.</i>" - Sparcrypt (Reddit)</p>

<br>

<p align="center">
  <a href="http://www.gnu.org/licenses/">
    <img src="https://img.shields.io/badge/License-GNU-blue.svg?longCache=true" alt="License">
  </a>
</p>

<div align="center">
  <sub>Created by
  <a href="https://twitter.com/trimstray">trimstray</a> and
  <a href="https://github.com/trimstray/test-your-sysadmin-skills/graphs/contributors">contributors</a>
</div>

<br>

****

<br>

:information_source: &nbsp;This project contains **278** test questions and answers that can be used as a test your knowledge or during an interview/exam for position such as **\*nix System Administrator**.

:heavy_check_mark: &nbsp;The answers are only **examples** and do not exhaust the whole topic. Most of them contains **useful resources** for a deeper understanding.

:warning: &nbsp;Questions marked **`***`** don't have answer yet or answer is incomplete - **make a pull request to add them**!

:traffic_light: &nbsp;If you find a question which doesn't make sense, or one of the answers doesn't seem right, or something seems really stupid; **please make a pull request**.

<br>

<p align="center">
  » <b><code><a href="https://github.com/trimstray/test-your-sysadmin-skills/issues">All suggestions are welcome</a></code></b> «
</p>

<br>

## Table of Contents

| <b><u>The type of chapter</u></b> | <b><u>Number of questions</u></b> | <b><u>Short description</u></b> |
| :---         | :---         | :---         |
| <b>[Introduction](#introduction)</b> |||
| :small_orange_diamond: [Simple Questions](#simple-questions) | 14 questions | Relaxed, fun and simple - are great for starting everything. |
| <b>[General Knowledge](#general-knowledge)</b> |||
| :small_orange_diamond: [Junior Sysadmin](#junior-sysadmin) | 64 questions | Reasonably simple and straight based on basic knowledge. |
| :small_orange_diamond: [Regular Sysadmin](#regular-sysadmin) | 91 questions | The mid level of questions if that you have sound knowledge. |
| :small_orange_diamond: [Senior Sysadmin](#senior-sysadmin) | 95 questions | Hard questions and riddles. Check it if you want to be good. |
| <b>[Secret Knowledge](#secret-knowledge)</b> ||
| :small_orange_diamond: [Guru Sysadmin](#guru-sysadmin) | 14 questions | Really deep questions are to get to know Guru Sysadmin. |

<br>

## <a name="introduction">Introduction</a>

### :diamond_shape_with_a_dot_inside: <a name="simple-questions">Simple Questions</a>

- <b>What did you learn this week?</b>
- <b>What excites or interests you about the sysadmin world?</b>
- <b>What is a recent technical challenge you experienced and how did you solve it?</b>
- <b>Tell me about the last major project you finished.</b>
- <b>Do you contribute to any open source projects?</b>
- <b>Describe the setup of your homelab.</b>
- <b>What personal achievement are you most proud of?</b>
- <b>Tell me about the biggest mistake you've made. How would you do it differently today?</b>
- <b>What software tools are you going to install the first day at a new job?</b>
- <b>Tell me about how you manage your knowledge database (e.g. wikis, files, portals).</b>
- <b>What news sources do you check daily? (sysadmin, security-related or other)</b>
- <b>Your NOC team has a new budget for sysadmin certifications. What certificate would you like and why?</b>
- <b>How do you interact with developers: *us vs. them* or *all pulling together with a different approach*?</b>
- <b>Which sysadmin question would you ask, if you were interviewing me, to know, how good I'm with non-standard situations?</b>

## <a name="general-knowledge">General Knowledge</a>

### :diamond_shape_with_a_dot_inside: <a name="junior-sysadmin">Junior Sysadmin</a>

###### System Questions (36)

<details>
<summary><b>Give some examples of Linux distribution names. What is your favorite Linux distro and why?</b></summary><br>
- Red Hat Enterprise Linux
- Fedora
- CentOS
- Debian
- Ubuntu
- Mint
- SUSE Linux Enterprise Server (SLES)
- SUSE Linux Enterprise Desktop (SLED)
- Slackware
- Arch
- Kali
- Backbox

My favorite Linux distribution:

- **Arch Linux**, which offers a nice minimalist base system on which one can build a custom operating system. The beauty of it too is that it has the Arch User Repository (AUR), which when combined with its official binary repositories allows it to probably have the largest repositories of any distribution. Its packaging process is also very simple, which means if one wants a package not in its official repositories or the AUR, it should be easy to make it for oneself.
- **Linux Mint**, which is also built from Ubuntu LTS releases, but features editions featuring a few different desktop environments, including Cinnamon, MATE and Xfce. Mint is quite polished and its aesthetics are rather appealing, I especially like its new icon theme, although I do quite dislike its GTK+ theme (too bland to my taste). I’ve also found a bug in its latest release Mint 19, that is getting quite irritating as I asked for with it over a fortnight ago on their forums and I have received no replies so far and it is a bug that makes my life on it more difficult.
- **Kali Linux**, is a Debian-based Linux distribution aimed at advanced Penetration Testing and Security Auditing. Kali contains several hundred tools which are geared towards various information security tasks, such as Penetration Testing, Security research, Computer Forensics and Reverse Engineering.

Useful resources:

- [List of Linux distributions](https://en.wikipedia.org/wiki/List_of_Linux_distributions)
- [What is your favorite Linux distro and why?](https://www.quora.com/What-is-your-favorite-Linux-distro-and-why)

</details>

<details>
<summary><b>What are the differences between Unix, Linux, BSD and GNU?</b></summary><br>

**GNU** isn't really an OS. It's more of a set of rules or philosophies that govern free software, that at the same time gave birth to a bunch of tools while trying to create an OS. So **GNU** tools are basically open versions of tools that already existed, but were reimplemented to conform to principals of open software. **GNU/Linux** is a mesh of those tools and the **Linux kernel** to form a complete OS, but there are other GNUs, e.g. **GNU/Hurd**.

**Unix** and **BSD** are "older" implementations of POSIX that are various levels of "closed source". **Unix** is usually totally closed source, but there are as many flavors of **Unix** as there are **Linux** (if not more). **BSD** is not usually considered "open", but it was considered to be very open when it was released. Its licensing also allowed for commercial use with far fewer restrictions than the more "open" licenses of the time allowed.

**Linux** is the newest of the four. Strictly speaking, it's "just a kernel"; however, in general, it's thought of as a full OS when combined with GNU Tools and several other core components.

The main governing differences between these are their ideals. **Unix**, **Linux**, and **BSD** have different ideals that they implement. They are all POSIX, and are all basically interchangeable. They do solve some of the same problems in different ways. So other then ideals and how they choose to implement POSIX standards, there is little difference.

For more info I suggest your read a brief article on the creation of **GNU**, **OSS**, **Linux**, **BSD**, and **UNIX**. They will be slanted towards their individual ideas, but those articles should give you a better idea of the differences.

Useful resources:

- [What is the difference between Unix, Linux, BSD and GNU? (original)](https://unix.stackexchange.com/questions/104714/what-is-the-difference-between-unix-linux-bsd-and-gnu)
- [The Great Debate: Is it Linux or GNU/Linux?](https://www.howtogeek.com/139287/the-great-debate-is-it-linux-or-gnulinux/)

</details>

<details>
<summary><b>What is a CLI? Tell me about your favorite CLI tools, tips and hacks.</b></summary><br>

**CLI** is an acronym for Command Line Interface or Command Language Interpreter. The command line is one of the most powerful ways to control your system/computer.

In Unix like systems, **CLI** is the interface by which a user can type commands for the system to execute. The **CLI** is very powerful, but is not very error-tolerant.

The **CLI** allows you to do manipulations with your system’s internals and with code in a much more fine-tuned way. It offers greater flexibility and control than a GUI regardless of what OS is used. Many programs that you might want to use in your software that are hosted on say Github also require running some commands on the **CLI** in order to get them running.

**My favorite tools**

- `screen` - free terminal multiplexer, I can start a session and My terminals will be saved even when you connection is lost, so you can resume later or from home
- `ssh` - the most valuable over-all command to learn, I can use it to do some amazing things:
  * mount a file system over the internet with `sshfs`
  * forward commands: runs against a `rsync` server with no `rsync` deamon by starting one itself via ssh
  * run in batch files: I can redirect the output from the remote command and use it within local batch file
- `vi/vim` - is the most popular and powerful text editor, it's universal, it's work very fast, even on large files
- `bash-completion` - contains a number of predefined completion rules for shell

**Tips & Hacks**

- searches the command history with `CTRL + R`
- `popd/pushd` and other shell builtins which allow you manipulate the directory stack
- editing keyboard shortcuts like a `CTRL + U`, `CTRL + E`
- combinations will be auto-expanded:
  * `!*` - all arguments of last command
  * `!!` - the whole of last command
  * `!ssh` - last command starting with ssh

Useful resources:

- [Command Line Interface Definition](http://www.linfo.org/command_line_interface.html)
- [What is your single most favorite command-line trick using Bash?](https://stackoverflow.com/questions/68372/what-is-your-single-most-favorite-command-line-trick-using-bash/69716)
- [What are your favorite command line features or tricks?](https://unix.stackexchange.com/questions/6/what-are-your-favorite-command-line-features-or-tricks)

</details>

<details>
<summary><b>What is your favorite shell and why?</b></summary><br>

**BASH** is my favorite. It’s really a preferential kind of thing, where I love the syntax and it just "clicks" for me. The input/output redirection syntax (`>>`, `<< 2>&1`, `2>`, `1>`, etc) is similar to C++ which makes it easier for me to recognize.

I also like the **ZSH** shell, because is much more customizable than **BASH**. It has the Oh-My-Zsh framework, powerful context based tab completion, pattern matching/globbing on steroids, loadable modules and more.

Useful resources:

- [Comparison of command shells](https://en.wikipedia.org/wiki/Comparison_of_command_shells)

</details>

<details>
<summary><b>How do you getting help the command line? ***</b></summary><br>

- `man` [commandname] can be used to see a description of a command (ex.: `man less`, `man cat`)

- `-h` or `--help` some programs will implement printing instructions when passed this parameter (ex.: `python -h` and `python --help`)

</details>

<details>
<summary><b>Your first 5 commands on a *nix server after login.</b></summary><br>

- `w` - a lot of great information in there with the server uptime
- `top` - you can see all running processes, then order them by CPU, memory utilization and more
- `netstat` - to know on what port and IP your server is listening on and what processes are using those
- `df` - reports the amount of available disk space being used by file systems
- `history` - tell you what was previously run by the user you are currently connected to

Useful resources:

- [First 5 Commands When I Connect on a Linux Server (original)](https://www.linux.com/blog/first-5-commands-when-i-connect-linux-server)

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
<summary><b>How do you get a list of logged-in users?</b></summary><br>

For a summary of logged-in users, including each login of a username, the terminal users are attached to, the date/time they logged in, and possibly the computer from which they are making the connection, enter:

```bash
# It uses /var/run/utmp and /var/log/wtmp files to get the details.
who
```

For extensive information, including username, terminal, IP number of the source computer, the time the login began, any idle time, process CPU cycles, job CPU cycles, and the currently running command, enter:

```bash
# It uses /var/run/utmp, and their processes /proc.
w
```

Also important for displays a list of last logged in users, enter:

```bash
# It uses /var/log/wtmp.
last
```

Useful resources:

- [4 Ways to Identify Who is Logged-In on Your Linux System](https://www.thegeekstuff.com/2009/03/4-ways-to-identify-who-is-logged-in-on-your-linux-system/)

</details>

<details>
<summary><b>What is the advantage of executing the running processes in the background? How can you do that?</b></summary><br>

The most significant advantage of executing the running process in the background is that you can do any other task simultaneously while other processes are running in the background. So, more processes can be completed in the background while you are working on different processes. It can be achieved by adding a special character `&` at the end of the command.

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
<summary><b>Before you can manage processes, you must be able to identify them. Which tools will you use? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Why is it bad to run commands as root user?</b></summary><br>

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
<summary><b>How to check memory stats and CPU stats?</b></summary><br>

You'd use `top/htop` for both. Using `free` and `vmstat` command we can display the physical and virtual memory statistics respectively. With the help of `sar` command we see the CPU utilization & other stats (but `sar` isn't even installed in most systems).

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
<summary><b>Where is my password stored on Linux/Unix?</b></summary><br>

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
<summary><b>How to recursively change permissions for all directories except files and for all files except directories?</b></summary><br>

To change all the directories e.g. to **755** (`drwxr-xr-x`):

```bash
find /opt/data -type d -exec chmod 755 {} \;
```

To change all the files e.g. to **644** (`-rw-r--r--`):

```bash
find /opt/data -type f -exec chmod 644 {} \;
```

Useful resources:

- [How do I set chmod for a folder and all of its subfolders and files? (original)](https://stackoverflow.com/questions/3740152/how-do-i-set-chmod-for-a-folder-and-all-of-its-subfolders-and-files?rq=1)

</details>

<details>
<summary><b>Every command fails with <code>command not found</code>. How to trace the source of the error and resolve it?</b></summary><br>

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
<summary><b>You typing <code>CTRL + C</code> but your script still running. How do you stop it? ***</b></summary><br>

To be completed.

Useful resources:

- [How to kill a script running in terminal, without closing terminal (Ctrl + C doesn't work)? (original)](https://askubuntu.com/questions/520107/how-to-kill-a-script-running-in-terminal-without-closing-terminal-ctrl-c-doe)
- [What's the difference between ^C and ^D for Unix/Mac OS X terminal?](https://superuser.com/questions/169051/whats-the-difference-between-c-and-d-for-unix-mac-os-x-terminal)

</details>

<details>
<summary><b>What is <code>grep</code> command? How to match multiple strings in the same line?</b></summary><br>

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
<summary><b>Explain file content commands along with the description.</b></summary><br>

- `head`: to check the starting of a file.
- `tail`: to check the ending of the file. It is the reverse of head command.
- `cat`: used to view, create, concatenate the files.
- `more`: used to display the text in the terminal window in pager form.
- `less`: used to view the text in the backward direction and also provides single line movement.

Useful resources:

- [Viewing text files from the shell prompt](https://access.redhat.com/documentation/en-US/Red_Hat_Enterprise_Linux/4/html/Step_by_Step_Guide/s1-viewingtext-terminal.html)

</details>

<details>
<summary><b>Explain SIGHUP, SIGINT, SIGKILL and SIGTERM Posix signals.</b></summary><br>

- **SIGHUP** - is sent to a process when its controlling terminal is closed. It was originally designed to notify the process of a serial line drop (a hangup). Many daemons will reload their configuration files and reopen their logfiles instead of exiting when receiving this signal.
- **SIGINT** - is sent to a process by its controlling terminal when a user wishes to interrupt the process. This is typically initiated by pressing `Ctrl+C`, but on some systems, the "delete" character or "break" key can be used.
- **SIGKILL** - is sent to a process to cause it to terminate immediately (kill). In contrast to **SIGTERM** and **SIGINT**, this signal cannot be caught or ignored, and the receiving process cannot perform any clean-up upon receiving this signal.
- **SIGTERM** - is sent to a process to request its termination. Unlike the **SIGKILL** signal, it can be caught and interpreted or ignored by the process. This allows the process to perform nice termination releasing resources and saving state if appropriate. **SIGINT** is nearly identical to **SIGTERM**.

Useful resources:

- [POSIX signals](https://dsa.cs.tsinghua.edu.cn/oj/static/unix_signal.html)
- [Introduction To Unix Signals Programming](http://titania.ctie.monash.edu.au/signals/)

</details>

<details>
<summary><b>What does <code>kill</code> command do?</b></summary><br>

In Unix and Unix-like operating systems, `kill` is a command used to send a signal to a process. By default, the message sent is the termination signal, which requests that the process exit. But `kill` is something of a misnomer; the signal sent may have nothing to do with process killing.

Useful resources:

- [Mastering the "Kill" Command in Linux](https://www.maketecheasier.com/kill-command-in-linux/)

</details>

<details>
<summary><b>What is the difference between <code>rm</code> and <code>rm -rf</code>?</b></summary><br>

`rm` only deletes the named files (and not directories). With `-rf` as you say:

- `-r`, `-R`, `--recursive` recursively deletes content of a directory, including hidden files and sub directories
- `-f`, `--force` ignore nonexistent files, never prompt

Useful resources:

- [What is the difference between `rm -r` and `rm -f`?](https://superuser.com/questions/1126206/what-is-the-difference-between-rm-r-and-rm-f)

</details>

<details>
<summary><b><code>archive.tgz</code> has ~30 GB. How do you list contents of it and extract only one file?</b></summary><br>

```bash
# list of content
tar tf archive.tgz

# extract file
tar xf archive.tgz filename
```

Useful resources:

- [List the contents of a tar or tar.gz file](https://www.cyberciti.biz/faq/list-the-contents-of-a-tar-or-targz-file/)
- [How to extract specific file(s) from tar.gz](https://unix.stackexchange.com/questions/61461/how-to-extract-specific-files-from-tar-gz)

</details>

<details>
<summary><b>Execute combine multiple shell commands in one line.</b></summary><br>

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
<summary><b>How can I sync two local directories?</b></summary><br>

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
<summary><b>Many basic maintenance tasks require you to edit config files. Explain ways to undo the changes you make.</b></summary><br>

- manually backup of a file before editing (with brace expansion like this: `cp filename{,.orig}`)
- manual copy of the directory structure where file is stored (e.g. `cp`, `rsync` or `tar`)
- make a backup of original file in your editor (e.g. set rules in your editor configuration file)
- the best solution is to use `git` (or any other version control) to keep track of configuration files (e.g. `etckeeper` for `/etc` directory)

Useful resources:

- [Backup file with .bak before filename extension](https://unix.stackexchange.com/questions/66376/backup-file-with-bak-before-filename-extension)
- [Is it a good idea to use git for configuration file version controlling?](https://superuser.com/questions/1037211/is-it-a-good-idea-to-use-git-for-configuration-file-version-controlling)

</details>

<details>
<summary><b>You have to find all files larger than 20M. How will you do this?</b></summary><br>

```bash
find / -type f -size +20M
```

Useful resources:

- [How can I find files that are bigger/smaller than x bytes?](https://superuser.com/questions/204564/how-can-i-find-files-that-are-bigger-smaller-than-x-bytes)

</details>

<details>
<summary><b>Why do we use <code>sudo su -</code> and not just <code>sudo su</code>?</b></summary><br>

`sudo` is in most modern Linux distributions where (but not always) the root user is disabled and has no password set. Therefore you cannot switch to the root user with `su` (you can try). You have to call `sudo` with root privileges: `sudo su`.

`su` just switches the user, providing a normal shell with an environment nearly the same as with the old user.

`su -` invokes a login shell after switching the user. A login shell resets most environment variables, providing a clean base.

Useful resources:

- [su vs sudo -s vs sudo -i vs sudo bash](https://unix.stackexchange.com/questions/35338/su-vs-sudo-s-vs-sudo-i-vs-sudo-bash)
- [Why do we use su - and not just su? (original)](https://unix.stackexchange.com/questions/7013/why-do-we-use-su-and-not-just-su)

</details>

<details>
<summary><b>How to find files that have been modified on your system in the past 60 minutes?</b></summary><br>

```bash
find / -mmin -60 -type f
```

Useful resources:

- [Get all files modified in last 30 days in a directory (orignal)](https://stackoverflow.com/questions/23070245/get-all-files-modified-in-last-30-days-in-a-directory)

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
<summary><b>How is a user’s default group determined? How would you change it? </b></summary><br>

```bash
useradd -m -g initial_group username
```

`-g/--gid`: defines the group name or number of the user's initial login group. If specified, the group name must exist; if a group number is provided, it must refer to an already existing group.

If not specified, the behaviour of useradd will depend on the `USERGROUPS_ENAB` variable contained in `/etc/login.defs`. The default behaviour (`USERGROUPS_ENAB yes`) is to create a group with the same name as the username, with **GID** equal to **UID**.

Useful resources:

- [How can I change a user's default group in Linux?](https://unix.stackexchange.com/questions/26675/how-can-i-change-a-users-default-group-in-linux)

</details>

<details>
<summary><b>What is your the best command line text editor for daily working and scripting? ***</b></summary><br>

To be completed.

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

###### Network Questions (23)

<details>
<summary><b>Draw me a simple network diagram: you have 20 systems, 1 router, 4 switches, 5 servers, and a small IP block. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What are the most important things to understand about the OSI (or any other) model?</b></summary><br>

The most important things to understand about the **OSI** (or any other) model are:

- we can divide up the protocols into layers
- layers provide encapsulation
- layers provide abstraction
- layers decouple functions from others

Useful resources:

- [OSI Model and Networking Protocols Relationship](https://networkengineering.stackexchange.com/questions/6380/osi-model-and-networking-protocols-relationship)

</details>

<details>
<summary><b>What is the difference between a VLAN and a subnet? Do you need a VLAN to setup a subnet?</b></summary><br>

**VLANs** and **subnets** solve different problems. **VLANs** work at Layer 2, thereby altering broadcast domains (for instance). Whereas **subnets** are Layer 3 in the current context.

**Subnet** - is a range of IP addresses determined by part of an address (often called the network address) and a subnet mask (netmask). For example, if the netmask is `255.255.255.0` (or `/24` for short), and the network address is `192.168.10.0`, then that defines a range of IP addresses `192.168.10.0` through `192.168.10.255`. Shorthand for writing that is `192.168.10.0/24`.

**VLAN** - a good way to think of this is "switch partitioning." Let's say you have an 8 port switch that is VLAN-able. You can assign 4 ports to one **VLAN** (say `VLAN 1`) and 4 ports to another **VLAN** (say `VLAN 2`). `VLAN 1` won't see any of `VLAN 2's` traffic and vice versa, logically, you now have two separate switches. Normally on a switch, if the switch hasn't seen a MAC address it will "flood" the traffic to all other ports. **VLANs** prevent this.

Subnet is nothing more than an IP address range of IP addresses that help hosts communicate over layer 2 and 3. Each subnet does not require its own **VLAN**. **VLANs** are implemented for isolation (are sandbox for layer two communication, no 2 systems of 2 different **VLANs** may communicate but it can be done through **Inter VLAN routing**), ease of management and security.

Useful resources:

- [What is the difference between a VLAN and a subnet? (original)](https://superuser.com/questions/353664/what-is-the-difference-between-a-vlan-and-a-subnet)
- [VLANS vs. subnets for network security and segmentation](https://networkengineering.stackexchange.com/questions/46899/vlans-vs-subnets-for-network-security-and-segmentation)

</details>

<details>
<summary><b>List 5 common network ports you should know.</b></summary><br>

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

Useful resources:

- [Red Hat Enterprise Linux 4: Security Guide - Common Ports](https://web.mit.edu/rhel-doc/4/RH-DOCS/rhel-sg-en-4/ch-ports.html)

</details>

<details>
<summary><b>What POP and IMAP are, and how to choose which of them you should implement? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>How to check default route and routing table?</b></summary><br>

Using the commands `netstat -nr`, `route -n` or `ip route show` we can see the default route and routing tables.

Useful resources:

- [How to check routes (routing table) in linux](https://howto.lintel.in/how-to-check-routes-routing-table-in-linux/)
- [FreeBSD Set a Default Route/Gateway](https://www.cyberciti.biz/faq/freebsd-setup-default-routing-with-route-command/)

</details>

<details>
<summary><b>What is the difference between 127.0.0.1 and localhost?</b></summary><br>

Well, the most likely difference is that you still have to do an actual lookup of localhost somewhere.

If you use `127.0.0.1`, then (intelligent) software will just turn that directly into an IP address and use it. Some implementations of `gethostbyname` will detect the dotted format (and presumably the equivalent IPv6 format) and not do a lookup at all.

Otherwise, the name has to be resolved. And there's no guarantee that your hosts file will actually be used for that resolution (first, or at all) so `localhost` may become a totally different IP address.

By that I mean that, on some systems, a local hosts file can be bypassed. The `host.conf` file controls this on Linux (and many other Unices).

If you use a Unix domain socket it'll be slightly faster than using TCP/IP (because of the less overhead you have). Windows is using TCP/IP as a default, whereas Linux tries to use a Unix Domain Socket if you choose localhost and TCP/IP if you take `127.0.0.1`.

Useful resources:

- [What is the difference between 127.0.0.1 and localhost?](https://stackoverflow.com/questions/7382602/what-is-the-difference-between-127-0-0-1-and-localhost)
- [localhost vs. 127.0.0.1](https://stackoverflow.com/questions/3715925/localhost-vs-127-0-0-1)

</details>

<details>
<summary><b>Which port is used for <code>ping</code> command?</b></summary><br>

`ping` uses **ICMP**, specifically **ICMP echo request** and **ICMP echo reply** packets. There is no 'port' associated with **ICMP**. Ports are associated with the two IP transport layer protocols, TCP and UDP. **ICMP**, TCP, and UDP are "siblings"; they are not based on each other, but are three separate protocols that run on top of IP.

**ICMP** packets are identified by the 'protocol' field in the IP datagram header. **ICMP** does not use either UDP or TCP communications services, it uses raw IP communications services. This means that the **ICMP** message is carried directly in an IP datagram data field. `raw` comes from how this is implemented in software, to create and send an **ICMP** message, one opens a `raw` socket, builds a buffer containing the **ICMP** message, and then writes the buffer containing the message to the raw socket.

The IP protocol value for **ICMP** is 1. The protocol field is part of the IP header and identifies what is in the data portion of the IP datagram.

However, you could use `nmap` to see whether ports are open or not:

```bash
nmap -p 80 example.com
```

Useful resources:

- [Ping Port Number](https://networkengineering.stackexchange.com/questions/42463/ping-port-number)
- [Is it possible to ping an address:port?](https://superuser.com/questions/769541/is-it-possible-to-ping-an-addressport)

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
<summary><b>Why won’t the hostnames resolve on your server? Fix this issue. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>How to resolve the domain name (using external dns) with CLI? Can IPs be resolved to domain names?</b></summary><br>

Examples for resolve IP address to domain name:

```bash
# with host command:
host domain.com 8.8.8.8

# with dig command:
dig @9.9.9.9 google.com

# with nslookup command:
nslookup domain.com 8.8.8.8
```

You can (sometimes) resolve an IP Address back to a hostname. IP Address can be stored against a **PTR** record. You can then do:

```bash
dig A <hostname>
```

To lookup the IPv4 address for a host, or:

```bash
dig AAAA <hostname>
```

To lookup the IPv6 address for a host, or:

```bash
dig PTR ZZZ.YYY.XXX.WWW.in-addr.arpa.
```

To lookup the hostname for IPv4 address `WWW.XXX.YYY.ZZZ` (note the octets are reversed), or:

```bash
dig PTR b.a.9.8.7.6.5.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.8.b.d.0.1.0.0.2.ip6.arpa.
```

Useful resources:

- [How can I resolve a hostname to an IP address in a Bash script?](https://unix.stackexchange.com/questions/20784/how-can-i-resolve-a-hostname-to-an-ip-address-in-a-bash-script)
- [How To Resolve IP Addresses To Domain Names?](https://superuser.com/questions/315687/how-to-resolve-ip-addresses-to-domain-names)

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
<summary><b>Why should you avoid <code>telnet</code> to administer a system remotely?</b></summary><br>

Modern operating systems have turned off all potentially insecure services by default. On the other hand, some vendors of network devices still allow to establish communication using the telnet protocol.

**Telnet** uses most insecure method for communication. It sends data across the network in plain text format and anybody can easily find out the password using the network tool.

In the case of **Telnet**, these include the passing of login credentials in plain text, which means anyone running a sniffer on your network can find the information he needs to take control of a device in a few seconds by eavesdropping on a **Telnet** login session.

Useful resources:

- [Telnet and SSH as a secure alternative](https://www.ssh.com/ssh/telnet)
- [How to telnet to an IP address on a specific port?](https://superuser.com/questions/339107/how-to-telnet-to-an-ip-address-on-a-specific-port)

</details>

<details>
<summary><b>What is the difference between <code>wget</code> and <code>curl</code>?</b></summary><br>

The main differences are: `wget's` major strong side compared to `curl` is its ability to download recursively. `wget` is command line only. `curl` supports FTP, FTPS, HTTP, HTTPS, SCP, SFTP, TFTP, TELNET, DICT, LDAP, LDAPS, FILE, POP3, IMAP, SMTP, RTMP and RTSP.

Useful resources:

- [What is the difference between curl and wget? (original)](https://unix.stackexchange.com/questions/47434/what-is-the-difference-between-curl-and-wget)

</details>

<details>
<summary><b>What is SSH and how does it work?</b></summary><br>

**SSH** stands for **Secure Shell**. It is a protocol that lets you drop from a server "A" into a shell session to a server "B". It allows you interact with your server "B".

An **SSH** connection to be established, the remote machine (server A) must be running a piece of software called an **SSH** daemon and the user's computer (server B) must have an **SSH** client.

The **SSH** daemon and **SSH** client listen for connections on a specific network port (default 22), authenticates connection requests, and spawns the appropriate environment if the user provides the correct credentials.

Useful resources:

- [Understanding the SSH Encryption and Connection Process](https://www.digitalocean.com/community/tutorials/understanding-the-ssh-encryption-and-connection-process)

</details>

<details>
<summary><b>Most tutorials suggest using SSH key authentication rather than password authentication. Why it is considered more secure?</b></summary><br>

An **SSH key** is an access credential in the SSH protocol. Its function is similar to that of user names and passwords, but the keys are primarily used for automated processes and for implementing single sign-on by system administrators and power users.

Instead of requiring a user's password, it is possible to confirm the client's identity by using asymmetric cryptography algorithms, with public and private keys.

If your SSH service only allows public-key authentication, an attacker needs a copy of a private key corresponding to a public key stored on the server.

If your SSH service allows password based authentication, then your Internet connected SSH server will be hammered day and night by bot-nets trying to guess user-names and passwords. The bot net needs no information, it can just try popular names and popular passwords. Apart from anything else this clogs your logs.

Useful resources:

- [Key-Based Authentication (Public Key Authentication)](http://www.crypto-it.net/eng/tools/key-based-authentication.html)
- [SSH password vs. key authentication](https://security.stackexchange.com/questions/33381/ssh-password-vs-key-authentication)

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

- [Building Internet Firewalls - Packet Filtering](http://web.deu.edu.tr/static/oreily/networking/firewall/ch06_01.htm)

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
<summary><b>What is the difference between a router and a gateway? What is the default gateway?</b></summary><br>

**Router** describes the general technical function (layer-3 forwarding) or a hardware device intended for that purpose, while gateway describes the function for the local segment (providing connectivity to elsewhere). You could also state that "_you set up a router as gateway_". Another term is hop which describes the forwarding in between subnets.

The term **default gateway** is used to mean the router on your LAN which has the responsibility of being the first point of contact for traffic to computers outside the LAN.

It's just a matter of perspective, the device is the same.

Useful resources:

- [Difference between router and gateway (orignal)](https://networkengineering.stackexchange.com/questions/51426/difference-between-router-and-gateway)

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
<summary><b>Why couldn't MAC addresses be used instead of IPv4/6 for networking?</b></summary><br>

The **OSI** model explains why it doesn't make sense to make routing, a **layer 3** concept, decisions based on a physical, **layer 2**, mechanism.

Modern networking is broken into many different layers to accomplish your end to end communication. Your network card (what is addressed by the mac address - physical address) needs to only be responsible for communicating with peers on it's physical network.

The communication that you are allowed to accomplish with your **MAC** address is going to be limited to other devices that reside within physical contact to your machine. On the internet, for example, you are not physically connected to each machine. That's why we make use of **TCP/IP** (a **layer 3**, logical address) mechanism when we need to communicate with a machine that we are not physically connected to.

**IP** is an arbitrary numbering scheme imposed in a hierarchical fashion on a group of computers to logically distinguish them as a group (that's what a subnet is). Sending messages between those groups is done by routing tables, themselves divided into multiple levels so that we don't have to keep track of every single subnet.

It's also pretty easy to relate this to another pair of systems. You have a State Issued ID Number, why would you need a mailing address if that ID number is already unique to just you? You need the mailing address because it's an arbitrary system that describes where the unique destination for communications to you should go.

On the other hand, the distribution of **MAC** addresses across the network is random and completely unrelated to topology. Routes grouping would be impossible, every router would need to keep track of routes for every single device that relays traffic trough it. That is what **layer 2** switches do, and that does not scale well beyond a certain number of hosts.

Useful resources:

- [Why couldn't MAC addresses be used instead of IPv4|6 for networking? (original)](https://serverfault.com/questions/410626/why-couldnt-mac-addresses-be-used-instead-of-ipv46-for-networking)

</details>

<details>
<summary><b>What is the smallest IPv4 subnet mask that can be applied to a network containing up to 30 devices?</b></summary><br>

Whether you have a standard `/24` VLAN for end users, a `/30` for point-to-point links, or something in between and subnet that must contain up to 30 devices works out to be a `/27` - or a subnet mask of `255.255.255.224`.

Useful resources:

- [How do you calculate the prefix, network, subnet, and host numbers?](https://networkengineering.stackexchange.com/questions/7106/how-do-you-calculate-the-prefix-network-subnet-and-host-numbers)
- [The slash after an IP Address - CIDR Notation](https://networkengineering.stackexchange.com/questions/3697/the-slash-after-an-ip-address-cidr-notation)
- [Why are there 3 ranges of private IPv4 addresses?](https://networkengineering.stackexchange.com/questions/32119/why-are-there-3-ranges-of-private-ipv4-addresses)
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

###### Devops Questions (5)

<details>
<summary><b>What is DevOps? Which is more important to the success of any DevOps community: how people communicate or the tools that you choose to deploy? ***</b></summary><br>

**DevOps** is a cohesive team that engages in both Development and Operations tasks, or it's individual Operations and Development teams that work very closely together. It's more of a "way" of working collaboratively with other departments to achieve common goals.

</details>

<details>
<summary><b>What is version control? Are your commit messages good looking?</b></summary><br>

It is a system that records changes to a file or set of files over time so that you can recall specific versions later. Version control systems consist of a central shared repository where teammates can commit changes to a file or set of file. Then you can mention the uses of version control.

Version control allows you to:

- revert files back to a previous state
- revert the entire project back to a previous state
- compare changes over time
- see who last modified something that might be causing a problem
- who introduced an issue and when

The seven rules of a great commit message:

- separate subject from body with a blank line
- limit the subject line to 50 characters
- capitalize the subject line
- do not end the subject line with a period
- use the imperative mood in the subject line
- wrap the body at 72 characters
- use the body to explain what and why vs. how

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
<summary><b>Explain some basic <code>docker</code> commands.</b></summary><br>

- `docker ps` - show running containers
- `docker ps -a` - show all containers
- `docker images` - show docker images
- `docker logs <container-id|container-name>` - get logs from container
- `docker network ls` - show all docker networks
- `docker volumes ls` - show all docker volumes
- `docker exec -it <container-id|container-name> bash` - execute bash in container with interactive shell

</details>

###### Cyber Security Questions (1)

<details>
<summary><b>What is a Security Misconfiguration?</b></summary><br>

**Security misconfiguration** is a vulnerability when a device/application/network is configured in a way which can be exploited by an attacker to take advantage of it. This can be as simple as leaving the default username/password unchanged or too simple for device accounts etc.

</details>

### :diamond_shape_with_a_dot_inside: <a name="regular-sysadmin">Regular Sysadmin</a>

###### System Questions (57)

<details>
<summary><b>What is your experience with the production environments? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Which distribution would you select for running a major web server? ***</b></summary><br>

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
<summary><b>Why is a load of 1.00 not ideal on a single-core machine?</b></summary><br>

The problem with a load of 1.00 is that you have no headroom. In practice, many sysadmins will draw a line at 0.70.

The "Need to Look into it" Rule of Thumb: 0.70 If your load average is staying above > 0.70, it's time to investigate before things get worse.

The "Fix this now" Rule of Thumb: 1.00. If your load average stays above 1.00, find the problem and fix it now. Otherwise, you're going to get woken up in the middle of the night, and it's not going to be fun.

Rule of Thumb: 5.0. If your load average is above 5.00, you could be in serious trouble, your box is either hanging or slowing way down, and this will (inexplicably) happen in the worst possible time like in the middle of the night or when you're presenting at a conference. Don't let it get there.

Useful resources:

- [Proper way of interpreting system load on a 4 core 8 thread processor](https://serverfault.com/questions/618130/proper-way-of-interpreting-system-load-on-a-4-core-8-thread-processor)
- [Understanding Linux CPU Load - when should you be worried?](http://blog.scoutapp.com/articles/2009/07/31/understanding-load-averages)

</details>

<details>
<summary><b>What does it mean when the effective user is root, but the real user ID is still your name?</b></summary><br>

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
<summary><b>Developer added cron job which generate massive log files. How do you prevent them from getting so big?</b></summary><br>

Using `logrotate` is the usual way of dealing with logfiles. But instead of adding content to `/etc/logrotate.conf` you should add your own job to `/etc/logrotate.d/`, otherwise you would have to look at more diffs of configuration files during release upgrades.

If it's actively being written to you don't really have much you can do by way of truncate. Your only options are to truncate the file:

```bash
: >/var/log/massive-logfile
```

It's very helpful, because it's truncate the file without disrupting the processes.

Useful resources:

- [How to Use logrotate to Manage Log Files](https://www.linode.com/docs/uptime/logs/use-logrotate-to-manage-log-files/)
- [System logging](https://www.ibm.com/developerworks/library/l-lpic1-108-2/index.html)

</details>

<details>
<summary><b>How the Linux kernel creates, manages and deletes the processes in the system? ***</b></summary><br>

To be completed.

Useful resources:

- [Linux Processes](https://www.tldp.org/LDP/tlk/kernel/processes.html)

</details>

<details>
<summary><b>Explain the selected information you can see in <code>top</code> and <code>htop</code>. How to diagnose load, high user time and out-of-memory problems with these tools? ***</b></summary><br>

To be completed.

Useful resources:

- [top explained visually](https://www.svennd.be/top-explained-visually/)
- [htop Explained Visually](https://codeahoy.com/2017/01/20/hhtop-explained-visually/)
- [Explanation of everything you can see in htop/top on Linux](https://peteris.rocks/blog/htop/)

</details>

<details>
<summary><b>How would you recognize a process that is hogging resources? </b></summary><br>

`top` works reasonably well, as long as you look at the right numbers.
- **M** Sorts by current resident memory usage
- **T** Sorts by total ( or cummulative) CPU usage
- **P** Sorts by current CPU usage (this is the default refresh)
- **?** Displays a usage summary for all top commands

This is very important information to obtain when problem solving why a computer process is running slowly and making decisions on what processes to kill/software to uninstall.

Useful resources:

- [How to find the process(es) which are hogging the machine](https://superuser.com/questions/326300/how-to-find-the-processes-which-are-hogging-the-machine)

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
<summary><b>When your server is booting up some errors appears on the console. How to examine boot messages and where are they stored?</b></summary><br>

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
<summary><b>Swap usage too high. What are the reasons for this and how to resolve swapping problems?</b></summary><br>

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
<summary><b>What is umask? How to set it permanently for a user?</b></summary><br>

On Linux and other Unix-like operating systems, new files are created with a default set of permissions. Specifically, a new file's permissions may be restricted in a specific way by applying a permissions "mask" called the `umask`. The `umask` command is used to set this mask, or to show you its current value.

Permanently change (set e.g. `umask 02`):

- `~/.profile`
- `~/.bashrc`
- `~/.zshrc`
- `~/.cshrc`

Useful resources:

- [What is Umask and How To Setup Default umask Under Linux?](https://www.cyberciti.biz/tips/understanding-linux-unix-umask-value-usage.html)

</details>

<details>
<summary><b>Explain the differences among the following umask values: 000, 002, 022, 027, 077 and 277.</b></summary><br>

<table style="width:100%">
  <tr>
    <th>Umask</th>
    <th>File result</th>
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

Useful resources:

- [What is Umask and How To Setup Default umask Under Linux?](https://www.cyberciti.biz/tips/understanding-linux-unix-umask-value-usage.html)

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
<summary><b>How does the sticky bit work? The <code>SUID/GUID</code> is the same?</b></summary><br>

This is probably one of my most irksome things that people mess up all the time. The **SUID/GUID** bit and the **sticky-bit** are 2 completely different things.

If you do a `man chmod` you can read about the **SUID** and **sticky-bits**.

**SUID/GUID**

What the above man page is trying to say is that the position that the x bit takes in the rwxrwxrwx for the user octal (1st group of rwx) and the group octal (2nd group of rwx) can take an additional state where the x becomes an s. When this occurs this file when executed (if it's a program and not just a shell script) will run with the permissions of the owner or the group of the file.

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
<summary><b>What does <code>LC_ALL=C</code> before command do? In what cases it will be useful?</b></summary><br>

`LC_ALL` is the environment variable that overrides all the other localisation settings. This sets all `LC_` type variables at once to a specified locale.

The main reason to set `LC_ALL=C` before command is that fine to simply get English output (general change the locale used by the command).

On the other hand, also important is to increase the speed of command execution with `LC_ALL=C` e.g. `grep` or `fgrep`. Using the `LC_ALL=C` locale increased our performance and brought command execution time down.

For example, if you set `LC_ALL=en_US.utf8` your system opened multiple files from the `/usr/lib/locale` directory. For `LC_ALL=C` a minimum amount of open and read operations is performed.

If you want to restore all your normal (original) locale settings for the session:

```bash
LC_ALL=
```

If `LC_ALL` does not work, try using `LANG` (if that still does not work, try `LANGUAGE`):

```bash
LANG=C date +%A
Monday
```

Useful resources:

- [What does LC_ALL=C do? (original)](https://unix.stackexchange.com/questions/87745/what-does-lc-all-c-do)
- [Speed up grep searches with LC_ALL=C](https://www.inmotionhosting.com/support/website/ssh/speed-up-grep-searches-with-lc-all)

</details>

<details>
<summary><b>During server configuration one of the steps is setting the permissions to the apps directories. What steps will you take and what mistakes to avoid?</b></summary><br>

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
<summary><b>What steps will be taken by init when you run <code>telinit 1</code> from run level 3? What will be the final result of this? If you use <code>telinit 6</code> instead of <code>reboot</code> command your server will be restarted? ***</b></summary><br>

To be completed.

Useful resources:

- [What differences it will make, if i use “telinit 6” instead of “reboot” command to restart my computer?](https://unix.stackexchange.com/questions/434560/what-differences-it-will-make-if-i-use-telinit-6-instead-of-reboot-command)

</details>

<details>
<summary><b>I have forgotten the root password! What do I do in BSD? What is the purpose of booting into single user mode?</b></summary><br>

Restart the system, type `boot -s` at the `Boot:` prompt to enter **single-user mode**.

At the question about the shell to use, hit `Enter` which will display a `#` prompt.

Enter `mount -urw /` to remount the root file system read/write, then run `mount -a` to remount all the file systems.

Run `passwd root` to change the root password then run `exit` to continue booting.

**Single user mode** should basically let you log in with root access & change just about anything. For example, you might use single-user mode when you are restoring a damaged master database or a system database, or when you are changing server configuration options (e.g. password recovery).

Useful resources:

- [FreeBSD Reset or Recover Root Password](https://www.cyberciti.biz/tips/howto-freebsd-reset-recover-root-password.html)
- [Single User Mode Definition](http://www.linfo.org/single_user_mode.html)

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
<summary><b>How to change the kernel parameters? What kernel options might you need to tune? ***</b></summary><br>

To set the kernel parameters in Unix-like, first edit the file `/etc/sysctl.conf` after making the changes save the file and run the command `sysctl -p`, this command will make the changes permanently without rebooting the machine.

Useful resources:

- [How to Change Kernel Runtime Parameters in a Persistent and Non-Persistent Way](https://www.tecmint.com/change-modify-linux-kernel-runtime-parameters/)

</details>

<details>
<summary><b>Explain <code>/proc</code> filesystem.</b></summary><br>

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
<summary><b>What is an inode? How to find file's inode number and how can you use it?</b></summary><br>

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
<summary><b><code>ls -l</code> shows file attributes as question marks. What does this mean and what steps will you take to remove "zombie" files?</b></summary><br>

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
<summary><b>To LVM or not to LVM. What benefits does it provide?</b></summary><br>

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
<summary><b>How to increase the size of LVM partition?</b></summary><br>

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
<summary><b>What is the proper way to upgrade/update a system in production? Do you automate these process? Do you set downtime for them? Write recommendations. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Your friend during configuration of the MySQL server asked you: <i>Should I run <code>sudo mysql_secure_installation</code> after installing mysql?</i> What do you think about it? </b></summary><br>

It would be better if you run command as it provides many security options like:

- You can set a password for root accounts
- You can remove root accounts that are accessible from outside the local host
- You can remove anonymous-user accounts
- You can remove the test database, which by default can be accessed by anonymous users

Useful resources:

- [What is Purpose of using mysql_secure_installation?](https://stackoverflow.com/questions/20760908/what-is-purpose-of-using-mysql-secure-installation)

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
<summary><b>During configuration HAProxy to working with Redis you get <code>General socket error (Permission denied)</code> from log. SELinux is enable. Explain basic SELinux troubleshooting in CLI. ***</b></summary><br>

Useful resources:

- [Basic SELinux Troubleshooting in CLI](https://access.redhat.com/articles/2191331)

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
<summary><b>How to run script as another user without password?</b></summary><br>

For example (with `visudo` command):

```bash
user1 ALL=(user2) NOPASSWD: /opt/scripts/bin/generate.sh
```

The command paths must be absolute! Then call `sudo -u user2 /opt/scripts/bin/generate.sh` from a user1 shell.

</details>

<details>
<summary><b>How to check if running as root in a bash script?</b></summary><br>

In a bash script, you have several ways to check if the running user is root.

As a warning, do not check if a user is root by using the root username. Nothing guarantees that the user with ID 0 is called root. It's a very strong convention that is broadly followed but anybody could rename the superuser another name.

I think the best way when using bash is to use `$EUID` because `$UID` could be changed and not reflect the real user running the script.

```bash
if (( $EUID != 0 )); then
  echo "Please run as root"
  exit
fi
```
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
<summary><b>You must run command that will be performed for a very long time. How to prevent killing this process after the ssh session drops?</b></summary><br>

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
<summary><b>How to reload PostgreSQL after configuration changes?</b></summary><br>

Solution 1:

```bash
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
<summary><b>You have added several aliases to <code>.profile</code>. How to reload shell without exit?</b></summary><br>

The best way is `exec $SHELL -l` because `exec` replaces the current process with a new one. Also good (but other) solution is `. ~/.profile`.

Useful resources:

- [How to reload .bash_profile from the command line?](https://stackoverflow.com/questions/4608187/how-to-reload-bash-profile-from-the-command-line)

</details>

<details>
<summary><b>How to exit without saving shell history?</b></summary><br>

```bash
kill -9 $$
```

or

```bash
unset HISTFILE && exit
```

Useful resources:

- [How do I close a terminal without saving the history?](https://unix.stackexchange.com/questions/25049/how-do-i-close-a-terminal-without-saving-the-history)

</details>

<details>
<summary><b>What is this UID 0 toor account? Have I been compromised?</b></summary><br>

**toor** is an alternative superuser account, where toor is root spelled backwards. It is intended to be used with a non-standard shell so the default shell for root does not need to change.

This is important as shells which are not part of the base distribution, but are instead installed from ports or packages, are installed in `/usr/local/bin` which, by default, resides on a different file system. If root's shell is located in `/usr/local/bin` and the file system containing `/usr/local/bin`) is not mounted, root will not be able to log in to fix a problem and will have to reboot into single-user mode in order to enter the path to a shell.

Some people use toor for day-to-day root tasks with a non-standard shell, leaving root, with a standard shell, for single-user mode or emergencies. By default, a user cannot log in using toor as it does not have a password, so log in as root and set a password for toor before using it to login.

Useful resources:

- [The root account (and toor)](https://administratosphere.wordpress.com/2007/10/04/the-root-account-and-toor/)

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
<summary><b>How to find out the dynamic libraries executables loads when run?</b></summary><br>

You can do this with `ldd` command:

```bash
ldd /bin/ls
```

</details>

<details>
<summary><b>You have the task of sync the testing and production environments. What steps will you take?</b></summary><br>

It's easy to get dragged down into bikeshedding about cloning environments and miss the real point:

- only production is production

and every time you deploy there you are testing a unique combination of deploy code + software + environment.

Every once in a while a good solution is regular cloning of the production servers to create testing servers. You can create instances with an exact copy of your production environment under a dev/test with snapshots, for example:

- generate a snapshot of production
- copy the snapshot to staging (or other)
- create a new disk using this snapshot

Sure, you can spin up clones of various system components or entire systems, and capture real traffic to replay offline (the gold standard of systems testing). But many systems are too big, complex, and cost-prohibitive to clone.

Before environment synchronization a good way is keeping track of every change that you make to the testing environment and provide a way for propagating this to the production environment, so that you do not skip any step and do it as smoothly as possible.

Also structure comparison tool or deploy scripts that update the testing environment from production environment is a good solution.

**Presync tasks**

First of all is informing developers and clients about not making changes on the test environment (if possible, disabling test domains that target this environment or set static pages with information about synchronization).

It is also important to make backup/snapshots of both environments.

**Database servers**

- sync/update system version (e.g. packages)
- create dump file from database on production db server
- import dump file on testing db server
- if necessary, syncs login permissions, roles, database permissions, open connections to the database and other

**Web/App servers**

- sync/update system version (e.g. packages)
- if necessary, updated kernel parameters, firewall rules and other
- sync/update configuration files of all running/important services
- sync/update user accounts (e.g. permissions) and their home directories
- deploy project from git/svn repository
- sync/update important directories existing in project, e.g. **static**, **asset** and other
- sync/update permissions for project directory
- remove/update all webhooks
- update cron jobs

**Others tasks**

- updated configurations of load balancers for testing domains and specific urls
- updated configurations of queues, session and storage instances

Useful resources:

- [Keeping testing and production server environments clean, in sync, and consistent](https://stackoverflow.com/questions/639668/keeping-testing-and-production-server-environments-clean-in-sync-and-consisten)

</details>

###### Network Questions (24)

<details>
<summary><b>Configure a virtual interface on your workstation. ***</b></summary><br>

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
<summary><b>Dev team reports an error: <code>POST http://ws.int/api/v1/Submit/ resulted in a 413 Request Entity Too Large</code>. What's wrong?</b></summary><br>

**Modify NGINX configuration file for domain**

Set correct `client_max_body_size` variable value:

```bash
client_max_body_size 20M;
```

Restart Nginx to apply the changes.

**Modify php.ini file for upload limits**

It’s not needed on all configurations, but you may also have to modify the PHP upload settings as well to ensure that nothing is going out of limit by php configurations.

Now find following directives one by one:

```bash
upload_max_filesize
post_max_size
```

and increase its limit to 20M, by default they are 8M and 2M:

```bash
upload_max_filesize = 20M
post_max_size = 20M
```

Finally save it and restart PHP.

Useful resources:

- [413 Request Entity Too Large in Nginx with client_max_body_size set](https://serverfault.com/questions/814767/413-request-entity-too-large-in-nginx-with-client-max-body-size-set)

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
<summary><b>How to check which ports are listening in my Linux Server?</b></summary><br>

Use the:

- `lsof -i`
- `ss -l`
- `netstat -atn` - for tcp
- `netstat -aun` - for udp
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
<summary><b>How to send an HTTP request using <code>telnet</code>?</b></summary><br>

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
<summary><b>How to allow traffic to/from specific IP with iptables?</b></summary><br>

For example:

```bash
/sbin/iptables -A INPUT -p tcp -s XXX.XXX.XXX.XXX -j ACCEPT
/sbin/iptables -A OUTPUT -p tcp -d  XXX.XXX.XXX.XXX -j ACCEPT
```

</details>

<details>
<summary><b>How to block abusive IP addresses with <code>pf</code> in OpenBSD?</b></summary><br>

The best way to do this is to define a table and create a rule to block the hosts, in `pf.conf`:

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
<summary><b>When does the web server like Apache or Nginx write info to log file? Before or after serving the request?</b></summary><br>

Both servers provides very comprehensive and flexible logging capabilities - for logging everything that happens on your server, from the initial request, through the URL mapping process, to the final resolution of the connection, including any errors that may have occurred in the process.

**Apache**

The Apache server access log records all requests processed by the server (after the request has been completed).

**Nginx**

NGINX writes information about client requests in the access log right after the request is processed.

Useful resources:

- [When does Apache log to access.log - before or after serving the request?](https://webmasters.stackexchange.com/questions/65566/when-does-apache-log-to-access-log-before-or-after-serving-the-request)
- [nginx log request before processing](https://serverfault.com/questions/693049/nginx-log-request-before-processing)

</details>

<details>
<summary><b>Analyse web server log and show only <code>5xx</code> http codes. What external tools do you use?</b></summary><br>

```bash
tail -n 100 -f /path/to/logfile | grep "HTTP/[1-2].[0-1]\" [5]"
```

Examples of http/https log management tools:

- **goaccess** - is an open source real-time web log analyzer and interactive viewer that runs in a terminal in *nix systems or through your browser
- **graylog** - is a free and open-source log management platform that supports in-depth log collection and analysis

Useful resources:

- [Best Log Management Tools: 51 Useful Tools for Log Management, Monitoring, Analytics, and More](https://stackify.com/best-log-management-tools/)

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

**CORS** allows the **Same Origin Policy** to be relaxed for a domain.

e.g. normally if the user logs into both `example.com` and `example.org`, the Same Origin Policy prevents `example.com` from making an AJAX request to `example.org/current_user/full_user_details` and gaining access to the response.

This is the default policy of the web and prevents the user's data from being leaked when logged into multiple sites at the same time.

Now with **CORS**, `example.org` could set a policy to say it will allow the origin `https://example.com` to read responses made by AJAX. This would be done if both `example.com` and `example.org` are ran by the same company and data sharing between the origins is to be allowed in the user's browser. It only affects the client-side of things, not the server-side.

**CSPs** on the other hand set a policy of what content can run on the current site. For example, if JavaScript can be executed inline, or which domains `.js` files can be loaded from. This can be beneficial to act as another line of defense against **XSS** attacks, where the attacker will try and inject script into the HTML page. Normally output would be encoded, however say the developer had forgotten only on one output field. Because the policy is preventing in-line script from executing, the attack is thwarted.

Useful resources:

- [What is the difference between CORS and CSPs? (original)](https://stackoverflow.com/questions/39488241/what-is-the-difference-between-cors-and-csps)
- [CSP, SRI and CORS](https://colorblindprogramming.com/csp-sri-and-cors)

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
<summary><b>What does a <code>tcpdump</code> do? How to capture only incoming traffic to your interface?</b></summary><br>

`tcpdump` is a most powerful and widely used command-line packets sniffer or package analyzer tool which is used to capture or filter TCP/IP packets that received or transferred over a network on a specific interface.

`tcpdump` puts your network card into promiscuous mode, which basically tells it to accept every packet it receives. It allows the user to see all traffic being passed over the network. Wireshark uses pcap to capture packets.

If you want to view only packets that come to your interface you should:

- `-Q in` - for Linux `tcpdump` version
- `-D in` - for BSD `tcpdump` version

Both params set send/receive direction direction for which packets should be captured.

```bash
tcpdump -nei eth0 -Q in host 192.168.252.125 and port 8080
```

</details>

###### Devops Questions (7)

<details>
<summary><b>Which are the top DevOps tools? Which tools have you worked on?</b></summary><br>

The most popular DevOps tools are mentioned below:

- **Git** : Version Control System tool
- **Jenkins** : Continuous Integration tool
- **Selenium** : Continuous Testing tool
- **Puppet**, **Chef**, **Ansible** : Configuration Management and Deployment tools
- **Nagios** : Continuous Monitoring tool
- **Docker** : Containerization tool

</details>

<details>
<summary><b>How do all these tools work together?</b></summary><br>

The most popular DevOps tools are mentioned below:

- Developers develop the code and this source code is managed by Version Control System tools like Git etc.
- Developers send this code to the Git repository and any changes made in the code is committed to this Repository
- Jenkins pulls this code from the repository using the Git plugin and build it using tools like Ant or Maven
- Configuration management tools like puppet deploys & provisions testing environment and then Jenkins releases this code on the test environment on which testing is done using tools like selenium
- Once the code is tested, Jenkins send it for deployment on the production server (even production server is provisioned & maintained by tools like puppet)
- After deployment It is continuously monitored by tools like Nagios
- Docker containers provides testing environment to test the build features

</details>

<details>
<summary><b>What are playbooks in Ansible?</b></summary><br>

Playbooks are Ansible’s configuration, deployment, and orchestration language.

They can describe a policy you want your remote systems to enforce, or a set of steps in a general IT process. Playbooks are designed to be human-readable and are developed in a basic text language.

At a basic level, playbooks can be used to manage configurations of and deployments to remote machines.

</details>

<details>
<summary><b>What is NRPE (Nagios Remote Plugin Executor) in Nagios?</b></summary><br>

The **NRPE** addon is designed to allow you to execute Nagios plugins on remote Linux/Unix machines. The main reason for doing this is to allow Nagios to monitor "local" resources (like CPU load, memory usage, etc.) on remote machines.

Since these public resources are not usually exposed to external machines, an agent like **NRPE** must be installed on the remote Linux/Unix machines.

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

<details>
<summary><b>Mention what are the advantages of using Redis? What is <code>redis-cli</code>? </b></summary><br>

- it provides high speed (exceptionally faster than others)
- it supports a server-side locking
- it has got lots of client lib
- it has got command level Atomic Operation (tx operation)
- supports for rich data types like hashes, sets, bitmaps

`redis-cli` is the **Redis** command line interface, a simple program that allows to send commands to **Redis**, and read the replies sent by the server, directly from the terminal.

Useful resources:

- [10 Advantages of Redis](https://dzone.com/articles/10-traits-of-redis)

</details>

###### Cyber Security Questions (4)

<details>
<summary><b>What is XSS, how will you mitigate it?</b></summary><br>

**Cross Site Scripting** is a JavaScript vulnerability in the web applications. The easiest way to explain this is a case when a user enters a script in the client side input fields and that input gets processed without getting validated. This leads to untrusted data getting saved and executed on the client side.

Countermeasures of XSS are input validation, implementing a CSP (Content security policy) and other.

</details>

<details>
<summary><b>HIDS vs NIDS and which one is better and why?</b></summary><br>

**HIDS** is host intrusion detection system and **NIDS** is network intrusion detection system. Both the systems work on the similar lines. It’s just that the placement in different. **HIDS** is placed on each host whereas **NIDS** is placed in the network. For an enterprise, **NIDS** is preferred as **HIDS** is difficult to manage, plus it consumes processing power of the host as well.

</details>

<details>
<summary><b>What is compliance?</b></summary><br>

Abiding by a set of standards set by a government/Independent party/organisation, e.g. an industry which stores, processes or transmits Payment related information needs to be complied with PCI DSS (Payment card Industry Data Security Standard). Other compliance examples can be an organisation complying with its own policies.

</details>

<details>
<summary><b>What is a WAF and what are its types?</b></summary><br>

**WAF** stands for web application firewall. It is used to protect the application by filtering legitimate traffic from malicious traffic. **WAF** can be either a box type or cloud based.

</details>

### :diamond_shape_with_a_dot_inside: <a name="senior-sysadmin">Senior Sysadmin</a>

###### System Questions (60)

<details>
<summary><b>Explain the current architecture you’re responsible for and point out where it’s scalable or fault-tolerant. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Tell me how code gets deployed in your current production. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What are the different types of kernels? Explain.</b></summary><br>

**Monolithic Kernels**

Earlier in this type of kernel architecture, all the basic system services like a process and memory management, interrupt handling etc were packaged into a single module in kernel space. This type of architecture led to some serious drawbacks like:

- the size of the kernel, which was huge
- poor maintainability, which means bug fixing or addition of new features resulted in recompilation of the whole kernel which could consume hours

In a modern day approach to monolithic architecture, the kernel consists of different modules which can be dynamically loaded and unloaded. This modular approach allows easy extension of OS's capabilities. With this approach, maintainability of kernel became very easy as only the concerned module needs to be loaded and unloaded every time there is a change or bug fix in a particular module.

Linux follows the monolithic modular approach.

**Microkernels**

This architecture majorly caters to the problem of ever growing size of kernel code which we could not control in the monolithic approach. This architecture allows some basic services like device driver management, protocol stack, file system etc to run in user space.

In this architecture, all the basic OS services which are made part of user space are made to run as servers which are used by other programs in the system through inter process communication (IPC).

Example: We have servers for device drivers, network protocol stacks, file systems, graphics, etc. Microkernel servers are essentially daemon programs like any others, except that the kernel grants some of them privileges to interact with parts of physical memory that are otherwise off limits to most programs.

**Hybrid Kernels (Modular Kernels)**

This is a combination of the above two, where the key idea is that Operating System services are in Kernel Space, and and there is no message passing, no performance overhead and no reliability benefits, of having services in user space.

This is used by Microsoft's NT kernels, all the way up to the latest Windows version.

Useful resources:

- [An Introduction to Kernels. The Heart of Computing Devices. (original)](https://keetmalin.wixsite.com/keetmalin/single-post/2017/08/24/An-Introduction-to-Kernels-The-Heart-of-Computing-Devices)

</details>

<details>
<summary><b>The program returns the error of the missing library. How to provide dynamically linkable libraries?</b></summary><br>

Environment variable `LD_LIBRARY_PATH` is a colon-separated set of directories where libraries should be searched for first, before the standard set of directories; this is useful when debugging a new library or using a nonstandard library for special purposes.

The best way to use `LD_LIBRARY_PATH` is to set it on the command line or script immediately before executing the program. This way the new `LD_LIBRARY_PATH` isolated from the rest of your system.

Example of use:

```bash
export LD_LIBRARY_PATH="/list/of/library/paths:/another/path" ./program
```

Useful resources:

- [How to correctly use LD_LIBRARY_PATH](http://wiredrevolution.com/system-administration/how-to-correctly-use-ld_library_path)

</details>

<details>
<summary><b>Write the most important rules for using root privileges safely for novice administrators. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is the advantage of synchronizing UID/GID across multiple systems?</b></summary><br>

There are several principle reasons why you want to co-ordinate the **user/UID** and **group/GID** management across your network.

The first is relatively obvious - it has to do with user and administrative convenience.

If each of your users are expected to have relatively uniform access to the systems throughout the network, then they'll expect the same username and password to work on each system that they are supposed to use. If they change their password they will expect that change to be global.

It also has a relationship with names and group names in Unix and Linux. They are mapped into numeric forms (**UID's** and **GID's** respectively). All file ownership (inodes) and processes use these numerics for all access and identity determination throughout the kernel and drivers. These numeric values are reverse mapped back to their corresponding principle symbolic representations (the names) by the utilities that display or process that information.

It is also recommended that you adopt a policy that **UID's** are not re-used. When a user leaves your organization you "retire" their **UID** (disabling their access by \*'ing out their passwd, removing them from the groups maps, setting their "shell" to some `/bin/denied` binary and their home directory to a secured _graveyard_ - I use `/home/.graveyard` on my systems).

The reason for this may not be obvious. However, if you are maintaining archival backups for several years (or indefinitely) you'll want to avoid any ambiguities and confusion that might result from restoring one (long gone) user's files and finding them owned by one of your new users.

Useful resources:

- [UID/GID Synchronization and Management (original)](https://linuxgazette.net/issue31/tag_uidgid.html)
- [What's the advantage of synchronizing UID/GID across Linux machines?](https://serverfault.com/questions/603987/whats-the-advantage-of-synchronizing-uid-gid-across-linux-machines)
- [How can I keep user accounts consistent across multiple machines?](https://unix.stackexchange.com/questions/141023/how-can-i-keep-user-acccounts-consistent-accross-multiple-machines)

</details>

<details>
<summary><b>What principles to follow for successful system performance tuning? ***</b></summary><br>

To be completed.

Useful resources:

- [An Introduction to Performance Tuning](https://www.oreilly.com/library/view/system-performance-tuning/059600284X/ch01.html)

</details>

<details>
<summary><b>Describe start-up configuration files and directory in BSD systems.</b></summary><br>

In BSD the primary start-up configuration file is `/etc/defaults/rc.conf`. System startup scripts such as `/etc/rc` and `/etc/rc.d` just include this file.

If you want to add other programs to system startup you need to change `/etc/rc.conf` file instead of `/etc/defaults/rc.conf`.

</details>

<details>
<summary><b>CPU spent the most of time for a IO operations to complete. Which tools do you use for diagnose what process(es) did exactly wait for IO? How to minimize IO wait time? ***</b></summary><br>

To be completed.

Useful resources:

- [Can anyone explain precisely what IOWait is?](https://serverfault.com/questions/12679/can-anyone-explain-precisely-what-iowait-is)

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
<summary><b>How to add new disk in Linux server without rebooting? How to rescan and add it in LVM?</b></summary><br>

To be completed.

Useful resources:

- [How to Add New Disk in Linux CentOS 7 Without Rebooting](https://linoxide.com/linux-how-to/add-new-disk-centos-7-without-rebooting/)

</details>

<details>
<summary><b>Explain each system calls used for process management in Linux.</b></summary><br>

There are some system calls for process management. These are as follows:

- `Fork()`: it is used to create a new process
- `Exec()`: it is used to execute a new process
- `Wait()`: it is used to make the process to wait
- `Exit()`: it is used to exit or terminate the process
- `Getpid()`: it is used to find the unique process ID
- `Getppid()`: it is used to check the parent process ID
- `Nice()`: it is used to bias the currently running process property

Useful resources:

- [System Calls](http://faculty.salina.k-state.edu/tim/ossg/Introduction/sys_calls.html)

</details>

<details>
<summary><b>Can’t mount the root file system. Why? ***</b></summary><br>

To be completed.

Useful resources:

- [What does "mounting a root file system" mean exactly?](https://superuser.com/questions/193918/what-does-mounting-a-root-file-system-mean-exactly)
- [How does a kernel mount the root partition?](https://unix.stackexchange.com/questions/9944/how-does-a-kernel-mount-the-root-partition)

</details>

<details>
<summary><b>You have to delete 100GB files. Which method will be the most optimal? ***</b></summary><br>

To be completed.

Useful resources:

- [Is there a way to delete 100GB file on Linux without thrashing IO/load?](https://serverfault.com/questions/336917/is-there-a-way-to-delete-100gb-file-on-linux-without-thrashing-io-load)
- [rm on a directory with millions of files](https://serverfault.com/questions/183821/rm-on-a-directory-with-millions-of-files)

</details>

<details>
<summary><b>Explain interrupts and interrupt handlers in Linux.</b></summary><br>

Here's a high-level view of the low-level processing. I'm describing a simple typical architecture, real architectures can be more complex or differ in ways that don't matter at this level of detail.

When an **interrupt** occurs, the processor looks if interrupts are masked. If they are, nothing happens until they are unmasked. When interrupts become unmasked, if there are any pending interrupts, the processor picks one.

Then the processor executes the interrupt by branching to a particular address in memory. The code at that address is called the **interrupt handler**. When the processor branches there, it masks interrupts (so the interrupt handler has exclusive control) and saves the contents of some registers in some place (typically other registers).

The interrupt handler does what it must do, typically by communicating with the peripheral that triggered the interrupt to send or receive data. If the interrupt was raised by the timer, the handler might trigger the OS scheduler, to switch to a different thread. When the handler finishes executing, it executes a special return-from-interrupt instruction that restores the saved registers and unmasks interrupts.

The interrupt handler must run quickly, because it's preventing any other interrupt from running. In the Linux kernel, interrupt processing is divided in two parts:

- The "top half" is the interrupt handler. It does the minimum necessary, typically communicate with the hardware and set a flag somewhere in kernel memory.
- The "bottom half" does any other necessary processing, for example copying data into process memory, updating kernel data structures, etc. It can take its time and even block waiting for some other part of the system since it runs with interrupts enabled.

Useful resources:

- [How is an Interrupt handled in Linux? (original)](https://unix.stackexchange.com/questions/5788/how-is-an-interrupt-handled-in-linux)
- [Interrupts and Interrupt Handlers](https://notes.shichao.io/lkd/ch7/)

</details>

<details>
<summary><b>What considerations come into play when designing a highly available application, both at the architecture level and the application level? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What fields are stored in an inode?</b></summary><br>

Within a POSIX system, a file has the following attributes which may be retrieved by the stat system call:

- **Device ID** (this identifies the device containing the file; that is, the scope of uniqueness of the serial number).
File serial numbers
- The **file mode** which determines the file type and how the file's owner, its group, and others can access the file
- A **link count** telling how many hard links point to the inode
- The **User ID** of the file's owner
- The **Group ID** of the file
- The **device ID** of the file if it is a device file.
- The **size of the file** in bytes
- **Timestamps** telling when the inode itself was last modified (ctime, inode change time), the file content last modified (mtime, modification time), and last accessed (atime, access time)
- The preferred **I/O block size**
- The **number of blocks** allocated to this file

Useful resources:

- [Inodes - an Introduction](http://www.grymoire.com/Unix/Inodes.html)

</details>

<details>
<summary><b>Ordinary users are able to read <code>/etc/passwd</code>. Is this a security hole? You know alternative password shadowing scheme?</b></summary><br>

Typically, the _hashed passwords_ are stored in `/etc/shadow` on most Linux systems:

```bash
-rw-r----- 1 root shadow 1349 2016-07-03 03:54 /etc/shadow
```

They are stored in `/etc/master.passwd` on BSD systems.

Programs that need to perform authentication still need to run with `root` privileges:

```bash
-rwsr-xr-x 1 root root 42792 2016-02-14 14:13 /usr/bin/passwd
```

If you dislike the `setuid root` programs and one single file containing all the hashed passwords on your system, you can replace it with the **Openwall TCB PAM module**. This provides every single user with their own file for storing their hashed password - as a result the number of `setuid root` programs on the system can be drastically reduced.

Useful resources:

- [Ordinary users are able to read /etc/passwd, is this a security hole? (original)](https://serverfault.com/questions/286654/ordinary-users-are-able-to-read-etc-passwd-is-this-a-security-hole/286657#286657)
- [tcb - the alternative to /etc/shadow](https://www.openwall.com/tcb/)
- [Why shadow your passwd file?](https://www.tldp.org/HOWTO/Shadow-Password-HOWTO-2.html)

</details>

<details>
<summary><b>What are some of the benefits of using systemd over SysV init? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>How do you run command every time a file is modified?</b></summary><br>

For example:

```bash
while inotifywait -e close_write filename ; do

  echo "changed" >> /var/log/changed

done
```

</details>

<details>
<summary><b>You need to copy a large amount of data. Explain the most effective way. ***</b></summary><br>

To be completed.

Useful resources:

- [Copying a large directory tree locally? cp or rsync?](https://serverfault.com/questions/43014/copying-a-large-directory-tree-locally-cp-or-rsync)

</details>

<details>
<summary><b>Tell me about the dangers and caveats of LVM.</b></summary><br>

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
<summary><b>Python dev team in your company have a dilemma what to choose: uwsgi or gunicorn. What are the pros/cons of each of the solutions from the admin's perspective? ***</b></summary><br>

To be completed.

Useful resources:

- [uWSGI vs. Gunicorn, or How to Make Python Go Faster than Node](https://blog.kgriffs.com/2012/12/18/uwsgi-vs-gunicorn-vs-node-benchmarks.html)

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
<summary><b>Difference between <code>nohup</code>, <code>disown</code> and <code>&</code>. What happens when using all together?</b></summary><br>

- `&` puts the job in the background, that is, makes it block on attempting to read input, and makes the shell not wait for its completion
- `disown` removes the process from the shell's job control, but it still leaves it connected to the terminal. One of the results is that the shell won't send it a **SIGHUP**. Obviously, it can only be applied to background jobs, because you cannot enter it when a foreground job is running
- `nohup` disconnects the process from the terminal, redirects its output to `nohup.out` and shields it from **SIGHUP**. One of the effects (the naming one) is that the process won't receive any sent **SIGHUP**. It is completely independent from job control and could in principle be used also for foreground jobs (although that's not very useful)

If you use all three together, the process is running in the background, is removed from the shell's job control and is effectively disconnected from the terminal.

Useful resources:

- [Difference between nohup, disown and & (original)](https://unix.stackexchange.com/questions/3886/difference-between-nohup-disown-and)

</details>

<details>
<summary><b>What is the main advantage of using <code>chroot</code>? When and  why do we use it? What is the purpose of the mount dev, proc, sys in a chroot environment?</b></summary><br>

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
<summary><b>One of the processes runs slowly. How to check how long has been running and which tools will you use?</b></summary><br>

To be completed.

Useful resources:

- [How to check how long a process has been running?](https://unix.stackexchange.com/questions/7870/how-to-check-how-long-a-process-has-been-running)
- [Linux how long a process has been running?](https://www.cyberciti.biz/faq/how-to-check-how-long-a-process-has-been-running/)
- [How to see system call that executed in current time by process?](https://stackoverflow.com/questions/42677724/how-to-see-system-call-that-executed-in-current-time-by-process)

</details>

<details>
<summary><b>What is a file descriptor in Linux?</b></summary><br>

In Unix and related computer operating systems, a file descriptor (FD, less frequently fildes) is an abstract indicator (handle) used to access a file or other input/output resource, such as a pipe or network socket. File descriptors form part of the POSIX application programming interface.

</details>

<details>
<summary><b>Which way of additionally feeding random entropy pool would you suggest for producing random passwords? How to improve it?</b></summary><br>

You should use `/dev/urandom`, not `/dev/random`. The two differences between `/dev/random` and `/dev/urandom` are:

 - `/dev/random` might be theoretically better _in the context of an information-theoretically secure algorithm_. This is the kind of algorithm which is secure against today's technology, and also tomorrow's technology, and technology used by aliens, and God's own iPad as well.

 - `/dev/urandom` will not block, while `/dev/random` may do so. `/dev/random` maintains a counter of "how much entropy it still has" under the assumption that any bits it has produced is a lost entropy bit. Blocking induces very real issues, e.g. a server which fails to boot after an automated install because it is stalling on its SSH server key creation.

So you want to use `/dev/urandom` and stop to worry about this entropy business.

The trick is that `/dev/urandom` never blocks, ever, even when it should: `/dev/urandom` is secure as long as it has received enough bytes of "initial entropy" since the last boot (32 random bytes are enough). A normal Linux installation will create a random seed (from `/dev/random`) upon installation, and save it on the disk. Upon each reboot, the seed will be read, fed into `/dev/urandom`, and a new seed immediately generated (from `/dev/urandom`) to replace it. Thus, this guarantees that `/dev/urandom` will always have enough initial entropy to produce cryptographically strong alea, perfectly sufficient for any mundane cryptographic job, including password generation.

Should any of these daemons require randomness when all available entropy has been exhausted, they may pause to wait for more, which can cause excessive delays in your application. Even worse, since most modern applications will either resort to using its own random seed created at program initialization, or to using `/dev/urandom` to avoid blocking, your applications will suffer from lower quality random data. This can affect the integrity of your secure communications, and can increase the chance of cryptoanalysis on your private data.

To check the amount of bytes of entropy currently available, use:

```bash
cat /proc/sys/kernel/random/entropy_avail
```

**rng-tools**

Fedora/Rh/Centos types: `sudo yum install rng-tools`.

On deb types: `sudo apt-get install rng-tools` to set it up.

Then run `sudo rngd -r /dev/urandom` before generating the keys.

**haveged**

Fedora/Rh/Centos types: `sudo yum install haveged` and add `/usr/local/sbin/haveged -w 1024` to `/etc/rc.local`.

On deb types: `sudo apt-get install haveged` and add `DAEMON_ARGS="-w 1024"` to `/etc/default/haveged` to set it up.

Then run `sudo rngd -r /dev/urandom` before generating the keys.

Useful resources:

- [Feeding /dev/random entropy pool? (original)](https://security.stackexchange.com/questions/89/feeding-dev-random-entropy-pool)
- [GPG does not have enough entropy](https://serverfault.com/questions/214605/gpg-does-not-have-enough-entropy)

</details>

<details>
<summary><b>What is the difference between <code>/sbin/nologin</code>, <code>/bin/false</code> and <code>/bin/true</code>?</b></summary><br>

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
<summary><b>What is the meaning of the error <code>maxproc limit exceeded by uid %i ...</code> in FreeBSD?</b></summary><br>

The FreeBSD kernel will only allow a certain number of processes to exist at one time. The number is based on the **kern.maxusers** variable.

**kern.maxusers** also affects various other in-kernel limits, such as network buffers. If the machine is heavily loaded, increase **kern.maxusers**. This will increase these other system limits in addition to the maximum number of processes.

To adjust the **kern.maxusers** value, see the File/Process Limits section of the Handbook. While that section refers to open files, the same limits apply to processes.

If the machine is lightly loaded but running a very large number of processes, adjust the **kern.maxproc** tunable by defining it in `/boot/loader.conf`.

</details>

<details>
<summary><b>How to read a file line by line and assigning the value to a variable?</b></summary><br>

For example:

```bash
while IFS='' read -r line || [[ -n "$line" ]] ; do
  echo "Text read from file: $line"
done < "/path/to/filename"
```

Explanation:

- `IFS=''` (or `IFS=`) prevents leading/trailing whitespace from being trimmed.
- `-r` prevents backslash escapes from being interpreted.
- `|| [[ -n $line ]]` prevents the last line from being ignored if it doesn't end with a `\n` (since  read returns a non-zero exit code when it encounters EOF).

Useful resources:

- [Read a file line by line assigning the value to a variable](https://stackoverflow.com/questions/10929453/read-a-file-line-by-line-assigning-the-value-to-a-variable)

</details>

<details>
<summary><b>The client reports that his site received a grade B in the ssllabs scanner. Prepare a checklist of best practice for ssl configuration. ***</b></summary><br>

Useful resources:

- [Getting a Perfect SSL Labs Score](https://michael.lustfield.net/nginx/getting-a-perfect-ssl-labs-score)
- [17 small suggestions how to improve ssllabs.com/ssltest/](https://community.qualys.com/thread/14023)
- [How do you score A+ with 100 on all categories on SSL Labs test with Let's Encrypt and Nginx?](https://stackoverflow.com/questions/41930060/how-do-you-score-a-with-100-on-all-categories-on-ssl-labs-test-with-lets-encry)

</details>

<details>
<summary><b>What does CPU jumps mean?</b></summary><br>

An OS is a very busy thing, particularly so when you have it doing something (and even when you aren't). And when we are looking at an active enterprise environment, something is always going on.

Most of this activity is "bursty", meaning processes are typically quiescent with short periods of intense activity. This is certainly true of any type of network-based activity (e.g. processing PHP requests), but also applies to OS maintenance (e.g. file system maintenance, page reclamation, disk I/O requests).

If you take a situation where you have a lot of such bursty processes, you get a very irregular and spiky CPU usage plot.

As `500 - Internal Server Error` says, the high number of context switches are going to make the situation even worse.

Useful resources:

- [What does "CPU jumps” mean? (original)](https://stackoverflow.com/questions/32185607/what-does-cpu-jumps-mean)

</details>

<details>
<summary><b>How do you trace a system call in Linux? Explain the possible methods.</b></summary><br>

**SystemTap**

This is the most powerful method. It can even show the call arguments:

Usage:

```bash
sudo apt-get install systemtap
sudo stap -e 'probe syscall.mkdir { printf("%s[%d] -> %s(%s)\n", execname(), pid(), name, argstr) }'
```

Then on another terminal:

```bash
sudo rm -rf /tmp/a /tmp/b
mkdir /tmp/a
mkdir /tmp/b
```

Sample output:

```bash
mkdir[4590] -> mkdir("/tmp/a", 0777)
mkdir[4593] -> mkdir("/tmp/b", 0777)
```

**`strace` with `-f|-ff` params**

You can use the `-f` and `-ff` option. Something like this:

```bash
strace -f -e trace=process bash -c 'ls; :
```

- `-f` : Trace child processes as they are created by currently traced processes as a result of the fork(2) system call.

- `-ff` : If the `-o` filename option is in effect, each processes trace is written to filename.pid where pid is the numeric process id of each process. This is incompatible with `-c`, since no per-process counts are kept.

**`ltrace -S` shows both system calls and library calls**

This awesome tool therefore gives even further visibility into what executables are doing.

**`ftrace` minimal runnable example**

Here goes a minimal runnable example. Run with `sudo`:

```bash
#!/bin/sh
set -eux

d=debug/tracing

mkdir -p debug
if ! mountpoint -q debug; then
  mount -t debugfs nodev debug
fi

# Stop tracing.
echo 0 > "${d}/tracing_on"

# Clear previous traces.
echo > "${d}/trace"

# Find the tracer name.
cat "${d}/available_tracers"

# Disable tracing functions, show only system call events.
echo nop > "${d}/current_tracer"

# Find the event name with.
grep mkdir "${d}/available_events"

# Enable tracing mkdir.
# Both statements below seem to do the exact same thing,
# just with different interfaces.
# https://www.kernel.org/static/html/v4.18/trace/events.html
echo sys_enter_mkdir > "${d}/set_event"
# echo 1 > "${d}/events/syscalls/sys_enter_mkdir/enable"

# Start tracing.
echo 1 > "${d}/tracing_on"

# Generate two mkdir calls by two different processes.
rm -rf /tmp/a /tmp/b
mkdir /tmp/a
mkdir /tmp/b

# View the trace.
cat "${d}/trace"

# Stop tracing.
echo 0 > "${d}/tracing_on"

umount debug
```

Sample output:

```bash
# tracer: nop
#
#                              _-----=> irqs-off https://sourceware.org/systemtap/documentation.html
#                             / _----=> need-resched
#                            | / _---=> hardirq/softirq
#                            || / _--=> preempt-depth
#                            ||| /     delay
#           TASK-PID   CPU#  ||||    TIMESTAMP  FUNCTION
#              | |       |   ||||       |         |
            mkdir-5619  [005] .... 10249.262531: sys_mkdir(pathname: 7fff93cbfcb0, mode: 1ff)
            mkdir-5620  [003] .... 10249.264613: sys_mkdir(pathname: 7ffcdc91ecb0, mode: 1ff)
```

One cool thing about this method is that it shows the function call for all processes on the system at once, although you can also filter PIDs of interest with `set_ftrace_pid`.

Useful resources:

- [How do I trace a system call in Linux? (original)](https://stackoverflow.com/questions/29840213/how-do-i-trace-a-system-call-in-linux)
- [Does ftrace allow capture of system call arguments to the Linux kernel, or only function names?](https://stackoverflow.com/questions/27608752/does-ftrace-allow-capture-of-system-call-arguments-to-the-linux-kernel-or-only)
- [How to trace just system call events with ftrace without showing any other functions in the Linux kernel?](https://stackoverflow.com/questions/52764544/how-to-trace-just-system-call-events-with-ftrace-without-showing-any-other-funct)
- [What system call is used to load libraries in Linux?](https://unix.stackexchange.com/questions/226524/what-system-call-is-used-to-load-libraries-in-linux)

</details>

<details>
<summary><b>How to remove all files except some from a directory?</b></summary><br>

Solution 1 - with `extglob`:

```bash
shopt -s extglob
rm !(textfile.txt|backup.tar.gz|script.php|database.sql|info.txt)
```

Solution 2 - with `find`:

```bash
find . -type f -not -name '*txt' -print0 | xargs -0 rm --
```

</details>

<details>
<summary><b>How to check if a string contains a substring in Bash?</b></summary><br>

You can use `*` (wildcards) outside a case statement, too, if you use double brackets:

```bash
string='some text'
if [[ $string = *"My long"* ]] ; then
  true
fi
```

</details>

<details>
<summary><b>Explain differences between <code>2>&-</code>, <code>2>/dev/null</code>, <code>|&</code>, <code>&>/dev/null</code> and <code>>/dev/null 2>&1</code>.</b></summary><br>

- a **number 1** = standard out (i.e. `STDOUT`)
- a **number 2** = standard error (i.e. `STDERR`)
- if a number isn't explicitly given, then **number 1** is assumed by the shell (bash)

First let's tackle the function of these.

`2>&-`

The general form of this one is `M>&-`, where **"M"** is a file descriptor number. This will close output for whichever file descriptor is referenced, i.e. **"M"**.

`2>/dev/null`

The general form of this one is `M>/dev/null`, where **"M"** is a file descriptor number. This will redirect the file descriptor, **"M"**, to `/dev/null`.

`2>&1`

The general form of this one is `M>&N`, where **"M"** & **"N"** are file descriptor numbers. It combines the output of file descriptors **"M"** and **"N"** into a single stream.

`|&`

This is just an abbreviation for `2>&1 |`. It was added in Bash 4.

`&>/dev/null`

This is just an abbreviation for `>/dev/null 2>&1`. It redirects file descriptor 2 (`STDERR`) and descriptor 1 (`STDOUT`) to `/dev/null`.

`>/dev/null`

This is just an abbreviation for `1>/dev/null`. It redirects file descriptor 1 (`STDOUT`) to `/dev/null`.

Useful resources:

- [Difference between 2>&-, 2>/dev/null, |&, &>/dev/null and >/dev/null 2>&1](https://unix.stackexchange.com/questions/70963/difference-between-2-2-dev-null-dev-null-and-dev-null-21)
- [Chapter 20. I/O Redirection](http://www.tldp.org/LDP/abs/html/io-redirection.html)

</details>

<details>
<summary><b>How to redirect stderr and stdout to different files in the same line?</b></summary><br>

Just add them in one line `command 2>> error 1>> output`.

However, note that `>>` is for appending if the file already has data. Whereas, `>` will overwrite any existing data in the file.

So, `command 2> error 1> output` if you do not want to append.

Just for completion's sake, you can write `1>` as just `>` since the default file descriptor is the output. so `1>` and `>` is the same thing.

So, `command 2> error 1> output` becomes, `command 2> error > output`.

</details>

<details>
<summary><b>Load averages are above 30 on a server with 24 cores but CPU shows around 70 percent idle. One of the common causes of this condition is? How to debug and fixed?</b></summary><br>

Requests which involve disk I/O can be slowed greatly if cpu(s) needs to wait on the disk to read or write data. I/O Wait, is the percentage of time the CPU has to wait on disk.

Lets looks at how we can confirm if disk I/O is slowing down application performance by using a few terminal command line tools (`top`, `atop` and `iotop`).

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
<summary><b>How to enforce authorization methods in SSH?</b></summary><br>

Force login with a password:

```bash
ssh -o PreferredAuthentications=password -o PubkeyAuthentication=no user@remote_host
```

Force login using the key:

```bash
ssh -o PreferredAuthentications=publickey -o PubkeyAuthentication=yes -i id_rsa user@remote_host
```

Useful resources:

- [How to force ssh client to use only password auth?](https://unix.stackexchange.com/questions/15138/how-to-force-ssh-client-to-use-only-password-auth)

</details>

<details>
<summary><b>Getting <code>Too many Open files</code> error for Postgres. How to resolve it?</b></summary><br>

Fixed the issue by reducing `max_files_per_process` e.g. to 200 from default 1000. This parameter is in `postgresql.conf` file and this sets the maximum number of simultaneously open files allowed to each server subprocess.

Usually people start to edit `/etc/security/limits.conf` file, but forget that this file only apply to the actively logged in users through the PAM system.

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
<summary><b>What is the difference between encryption and hashing?</b></summary><br>

**Hashing**: Finally, hashing is a form of cryptographic security which differs from **encryption** whereas **encryption** is a two step process used to first encrypt and then decrypt a message, **hashing** condenses a message into an irreversible fixed-length value, or hash.

</details>

<details>
<summary><b>Should the root certificate go on the server?</b></summary><br>

**Self-signed root certificates** need not/should not be included in web server configuration. They serve no purpose (clients will always ignore them) and they incur a slight performance (latency) penalty because they increase the size of the SSL handshake.

If the client does not have the root in their trust store, then it won't trust the web site, and there is no way to work around that problem. Having the web server send the root certificate will not help - the root certificate has to come from a trusted 3rd party (in most cases the browser vendor).

Useful resources:

- [SSL root certificate optional?](https://security.stackexchange.com/questions/65332/ssl-root-certificate-optional)

</details>

<details>
<summary><b>How to log all commands run by root on production servers?</b></summary><br>

`auditd` is the correct tool for the job here:

1. Add these 2 lines to `/etc/audit/audit.rules`:

```bash
-a exit,always -F arch=b64 -F euid=0 -S execve
-a exit,always -F arch=b32 -F euid=0 -S execve
```

These will track all commands run by root (euid=0). Why two rules? The execve syscall must be tracked in both 32 and 64 bit code.

2. To get rid of `auid=4294967295` messages in logs, add `audit=1` to the kernel's cmdline (by editing `/etc/default/grub`)

3. Place the line

```bash
session  required                pam_loginuid.so
```

in all PAM config files that are relevant to login (`/etc/pam.d/{login,kdm,sshd}`), but not in the files that are relevant to su or sudo. This will allow auditd to get the calling user's uid correctly when calling sudo or su.

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

Now read `/var/log/audit/auditd.log` for show what has been logged in.

Useful resources:

- [Log all commands run by admins on production servers](https://serverfault.com/questions/470755/log-all-commands-run-by-admins-on-production-servers)

</details>

<details>
<summary><b>How to prevent <code>dd</code> from freezing system?</b></summary><br>

Try using ionice:

```bash
ionice -c3 dd if=/dev/zero of=z
```

This start the `dd` process with the "idle" IO priority: it only gets disk time when no other process is using disk IO for a certain amount of time.

Of course this can still flood the buffer cache and cause freezes while the system flushes out the cache to disk. There are tunables under `/proc/sys/vm/` to influence this, particularly the `dirty_*` entries.

</details>

<details>
<summary><b>How to limit processes to not exceed more than X% of CPU usage?</b></summary><br>

**nice/renice**

nice is a great tool for 'one off' tweaks to a system:

```bash
nice COMMAND
```

**cpulimit**

cpulimit if you need to run a CPU intensive job and having free CPU time is essential for the responsiveness of a system:

```bash
cpulimit -l 50 COMMAND
```

**cgroups**

cgroups apply limits to a set of processes, rather than to just one:

```bash
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
<summary><b>Other admin trying to debug a server accidentally typed: <code>chmod -x /bin/chmod</code>. How to reset permissions back to default?</b></summary><br>

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

Useful resources:

- [What can you do when you can't chmod chmod?](https://www.networkworld.com/article/3002286/operating-systems/what-can-you-do-when-you-cant-chmod-chmod.html)

</details>

<details>
<summary><b><code>grub></code> vs <code>grub-rescue></code>. Explain.</b></summary><br>

- `grub>` - this is the mode to which it passes if you find everything you need to run the system in addition to the configuration file. With this mode, we have access to most (if not all) modules and commands. This mode can be called from the menu by pressing the 'c' key
- `grub-rescue` - this is the mode to which it passes if it is impossible to find its own directory (especially the directory with modules and additional commands, e.g. directory `/boot/grub/i386-pc`), if its contents are damaged or if no normal module is found, contains only basic commands

</details>

<details>
<summary><b>How to check whether the private key and the certificate match?</b></summary><br>

```bash
(openssl rsa -noout -modulus -in private.key | openssl md5 ; openssl x509 -noout -modulus -in certificate.crt | openssl md5) | uniq
```

</details>

<details>
<summary><b>What steps to add a user to a system without using <code>useradd</code>/<code>adduser</code>?</b></summary><br>

1. Add an entry of user details in <code>/etc/passwd</code> with `vipw`:

```bash
# username:password:UID:GID:Comments:Home_Directory:Login Shell
user:x:501:501:test user:/home/user:/bin/bash
```

  > Be careful with the syntax. Do not edit directly with an editor. `vipw` locks the file, so that other commands won't try to update it at the same time.

2. You will have to create a group with same name in <code>/etc/group</code> with `vigr` (similar tool for `vipw`):

```bash
user:x:501:
```

3. Assign a password to the user:

```bash
passwd user
```

4. Create the home directory of the user with mkdir:

```bash
mkdir -m 0700 /home/user
```

5. Copy the files from `/etc/skel` to the new home directory:

```bash
rsync -av --delete /etc/skel/ /home/user
```

6. Fix ownerships and permissions with `chown` and `chmod`:

```bash
chown -R user:user /home/user
chmod -R go-rwx /home/user
```

Useful resources:

- [What steps to add a user to a system without using useradd/adduser?](https://unix.stackexchange.com/questions/153225/what-steps-to-add-a-user-to-a-system-without-using-useradd-adduser)

</details>

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
<summary><b>Write a simple bash script (or pair of scripts) to backup and restore your system. ***</b></summary><br>

To be completed.

</details>

###### Network Questions (24)

<details>
<summary><b>Create SPF records for your site to help control spam. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is the difference between an authoritative and a nonauthoritative answer to a DNS query? ***</b></summary><br>

To be completed.

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
<summary><b>Explore the current MTA configuration at your site. What are some of the special features of the MTA that are in use? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>How to find a domain based on the IP address? What techniques/tools can you use? ***</b></summary><br>

To be completed.

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

<details>
<summary><b>How do you do load testing and capacity planning for websites? ***</b></summary><br>

To be completed.

Useful resources:

- [How do you do load testing and capacity planning for web sites? (original)](https://serverfault.com/questions/350454/how-do-you-do-load-testing-and-capacity-planning-for-web-sites)
- [Can you help me with my capacity planning?](https://serverfault.com/questions/384686/can-you-help-me-with-my-capacity-planning)
- [How do you do load testing and capacity planning for databases?](https://serverfault.com/questions/350458/how-do-you-do-load-testing-and-capacity-planning-for-databases)

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
<summary><b>Does having Varnish in front of your website/app mean you don't need to care about load balancing or redundancy?</b></summary><br>

It depends. Varnish is a cache server, so its purpose is to cache contents and to act as a reverse proxy, to speed up retrieval of data and to lessen the load on the webserver.
Varnish can be also configured as a load-balancer for multiple web servers, but if we use just one Varnish server, this will become our single point of failure on our infrastructure.

A better solution to ensure load-balancing or redundancy will be a cluster of at least two Varnish instances, in active-active mode or active-passive mode.

</details>

<details>
<summary><b>What are hits, misses, and hit-for-pass in Varnish Cache?</b></summary><br>

A **hit** is a request which is successfully served from the cache, a **miss** is a request that goes through the cache but finds an empty cache and therefore has to be fetched from the origin, the **hit-for-pass** comes in when Varnish Cache realizes that one of the objects it has requested is uncacheable and will result in a pass.

Useful resources:

- [VCL rules for hits](https://book.varnish-software.com/4.0/chapters/VCL_Subroutines.html#vcl-vcl-hit)
- [VCL rules for hit-for-pass](https://book.varnish-software.com/4.0/chapters/VCL_Subroutines.html#hit-for-pass)
- [Example of the use](https://book.varnish-software.com/4.0/chapters/VCL_Basics.html#vcl-backend-response)

</details>

<details>
<summary><b>What is a reasonable TTL for cached content given the following parameters? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Developer says: <i><code>htaccess</code> is full of magic and it should be used</i>. What is your opinion about using <code>htaccess</code> files? What are the consequences for web application?</b></summary><br>

`.htaccess` files were born out of an era when shared hosting was common­place:

- sysadmins needed a way to allow multiple clients to access their server under different accounts, with different configurations for their web­sites.

The `.htaccess` file allowed them to modify how Apache works without having access to the entire server. These files can reside in any and every directory in the directory tree of the website and provide features to the directory and the files and folders inside it.

**It’s horrible for performance**

For `.htaccess` to work Apache needs to check EVERY directory in the requested path for the existence of a `.htaccess` file and if it exists it reads EVERY one of them and parses it. This happens for EVERY request. Remember that the second you change that file, it’s effective. This is because Apache reads it every time.

Every single request the web­server handles - even for the lowliest `.png` or `.css` file - causes Apache to:

- look for a `.htaccess` file in the directory of the current request
- then look for a `.htaccess` file in every directory from there up to the server root
- coalesce all of these `.htaccess` files together
- reconfigure the web­server using the new settings
- finally, deliver the file

Every web­page can generate dozens of requests. This is over­head you don’t need, and what’s more, it’s completely unnecessary.

**Security and permission loss**

Allowing individual users to modify the configuration of a server using `.htaccess` can cause security concerns if not taken care properly. If you add any directive in the `.htaccess` file, it will be considered as they are added to Apache configuration file.

This means it may be possible for non-admins to write these files and thus 'undo' all of your security. If you need to do something that is temporary, `.htaccess` is a good place to do it, if you need to do something more permanent, just put it in your `/etc/apache/sites-available/site.conf` (or `httpd.conf` or whatever your server calls).

**Summary**

You should avoid using `.htaccess` files completely if you have access to httpd main server config file. If it worked in `.htaccess`, it will work in your virtual host `.conf` file as well.

If you cannot avoid using `.htaccess` files, you should follow these rules.

- use only one `.htaccess` file or as few as possible
- place the `.htaccess` file in the site root directory
- keep your `.htaccess` file short and simple

Useful resources:

- [Like Apache: .htaccess](https://www.nginx.com/resources/wiki/start/topics/examples/likeapache-htaccess/)
- [Don't Use .htaccess Unless You Must](https://www.danielmorell.com/guides/htaccess-seo/basics/dont-use-htaccess-unless-you-must)

</details>

<details>
<summary><b>How to test connection to remote host with and without SNI? In which cases it is useful?</b></summary><br>

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
<summary><b>How to prevent processing requests in web server with undefined server names? No defined default server name rule can be security issue? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is the proper way to test NFS performance?
</b></summary><br>

The best benchmark is always "the application(s) that you normally use". The load on a NFS system when you have 20 people simultaneously compiling a Linux kernel is completely different from a bunch of people logging in at the same time or the accounts uses as "home directories for the local web-server".

But we have some good tools for testing this.

- <b>boonie</b> - a classical performances evaluation tool tests. The main program tests database type access to a single file (or a set of files if you wish to test more than 1G of storage), and it tests creation, reading, and deleting of small files which can simulate the usage of programs such as Squid, INN, or Maildir format email.
- <b>DBench</b> - was written to allow independent developers to debug and test SAMBA. It is heavily inspired of the original SAMBA tool.
- <b>IOZone</b> - performance tests suite. POSIX and 64 bits compliant. This tests is the file system test from the L.S.E. Main features: POSIX async I/O, Mmap() file I/O, Normal file I/O Single stream measurement, Multiple stream measurement, Distributed file server measurements (Cluster) POSIX pthreads, Multi-process measurement selectable measurements with fsync, O_SYNC Latency plots.

</details>

<details>
<summary><b>You need to block several IP addresses from the same subnet. Which is more efficient for the system to traverse the iptables rule set or the black-hole route?</b></summary><br>

If you have a system with thousands of routes defined in the routing table and nothing in the iptables rules than it might actually be more efficient to input an iptables rule.

In most systems however the routing table is fairly small, in cases like this it is actually more efficient to use null routes. This is especially true if you already have extensive iptables rules in place.

Assuming you're blocking based on source address and not destination, then doing the **DROP** in **raw/PREROUTING** would work well as you would essentially be able to drop the packet before any routing decision is made.

Remember however that iptables rules are essentially a linked-list and for optimum performance when blocking a number of addresses you should use an `ipset`.

On the other hand if blocking by destination, there is likely little difference between blocking at the routing table vs iptables **EXCEPT** if source IPs are spoofed in which case the blackholed entries may consume routing cache resources; in this case, **raw/PREROUTING** remains preferable.

Your outgoing route isn't going to matter until you try to send a packet back to the attacker. By that time you will have already incurred most of the cost of socket setup and may even have a thread blocking waiting for the kernel to conclude you have no route to host, plus whatever error handling your server process does when it concludes there's a network problem.

iptables or another firewall will allow you to block the incoming traffic and discard it before it reaches the daemon process on your server. It seems clearly superior in this use case.

```bash
iptables -A INPUT -s 192.168.200.0/24 -j DROP
```

When you define a route on a Linux/Unix system it tells the system in order to communicate with the specified IP address you will need to route your network communication to this specific place.

When you define a null route it simply tells the system to drop the network communication that is designated to the specified IP address. What this means is any TCP based network communication will not be able to be established as your server will no longer be able to send an SYN/ACK reply. Any UDP based network communication however will still be received; however your system will no longer send any response to the originating IP.

While iptables can accept tens of thousands of rules in a chain, the chains are walked sequentially until a match is found on every packet. So, lots of rules can lead to the system spending amazing amounts of CPU time walking through the rules.

The routing rules are much simpler than iptables. With iptables, a match can be based on many different variables including protocols, source and destination packets, and even other packets that were sent before the current packet.

In routing, all that matters is the remote IP address, so it's very easy to optimize. Also, many systems have a lot of routing rules. A typical system may only have 5 or 10, but something that's acting as a BGP router can have tens of thousands. So, for a very long time there have been extensive optimizations in selecting the right route for a particular packet.

In less technical terms this means your system will receive data from the attackers but no longer respond to it.

```bash
ip route add blackhole 192.168.200.0/24
```

or

```bash
ip route add 192.168.200.0/24 via 127.0.0.1
```

Useful resources:

- [The difference between iptables DROP and null-routing.](https://www.tummy.com/blogs/2006/07/27/the-difference-between-iptables-drop-and-null-routing/)

</details>

<details>
<summary><b>How to run <code>scp</code> with a second remote host?</b></summary><br>

With `ssh`:

```bash
ssh user1@remote1 'ssh user2@remote2 "cat file"' > file
```

With `tar` (with compression):

```bash
ssh user1@remote1 'ssh user2@remote2 "cd path2; tar cj file"' | tar xj
```

With `ssh` and port forwarding tunnel:

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
<summary><b>What types of dns cache working when you type api.example.com in your browser and press return?</b></summary><br>

Browser checks if the domain is in its cache (to see the DNS Cache in Chrome, go to `chrome://net-internals/#dns`). When this cache fails, it simply asks the OS to resolve the domain.

The OS resolver has it's own cache which it will check. If it fails this, it resorts to asking the OS configured DNS servers.

The OS configured DNS servers will typically be configured by DHCP from the router where the DNS servers are likely to be the ISP's DNS servers configured by DHCP from the internet gateway to the router.

In the event the router has it's own DNS servers, it may have it's own cache otherwise you should be directed straight to your ISP's DNS servers most typically as soon as the OS cache was found to be empty.

Useful resources:

- [What happens when...](https://github.com/alex/what-happens-when)
- [DNS Explained - How Your Browser Finds Websites](https://scotch.io/tutorials/dns-explained-how-your-browser-finds-websites)
- [Firefox invalidate dns cache](https://stackoverflow.com/questions/13063496/firefox-invalidate-dns-cache)

</details>

<details>
<summary><b>What is the difference between <code>Cache-Control: max-age=0</code> and <code>Cache-Control: no-cache</code>?</b></summary><br>

**When sent by the origin server**

`max-age=0` simply tells caches (and user agents) the response is stale from the get-go and so they SHOULD revalidate the response (e.g. with the If-Not-Modified header) before using a cached copy, whereas, `no-cache` tells them they MUST revalidate before using a cached copy.

In other words, caches may sometimes choose to use a stale response (although I believe they have to then add a Warning header), but `no-cache` says they're not allowed to use a stale response no matter what. Maybe you'd want the SHOULD-revalidate behavior when baseball stats are generated in a page, but you'd want the MUST-revalidate behavior when you've generated the response to an e-commerce purchase.

**When sent by the user agent**

If a user agent sends a request with `Cache-Control: max-age=0` (aka. "end-to-end revalidation"), then each cache along the way will revalidate its cache entry (e.g. with the If-Not-Modified header) all the way to the origin server. If the reply is then 304 (Not Modified), the cached entity can be used.

On the other hand, sending a request with `Cache-Control: no-cache` (aka. "end-to-end reload") doesn't revalidate and the server MUST NOT use a cached copy when responding.

</details>

<details>
<summary><b>What are the security risks of setting <code>Access-Control-Allow-Origin</code>?</b></summary><br>

By responding with <code>Access-Control-Allow-Origin: *</code>, the requested resource allows sharing with every origin. This basically means that any site can send an XHR request to your site and access the server’s response which would not be the case if you hadn’t implemented this CORS response.

So any site can make a request to your site on behalf of their visitors and process its response. If you have something implemented like an authentication or authorization scheme that is based on something that is automatically provided by the browser (cookies, cookie-based sessions, etc.), the requests triggered by the third party sites will use them too.

</details>

<details>
<summary><b>Create a single-use TCP or UDP proxy with <code>netcat</code>.</b></summary><br>

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
<summary><b>Explain 3 techniques for avoiding firewalls with <code>nmap</code>.</b></summary><br>

**Use Decoy addresses**

```bash
# Generates a random number of decoys.
nmap -D RND:10 [target]

# Manually specify the IP addresses of the decoys.
nmap -D decoy1,decoy2,decoy3
```

In this type of scan you can instruct Nmap to spoof packets from other hosts.In the firewall logs it will be not only our IP address but also and the IP addresses of the decoys so it will be much harder to determine from which system the scan started.

**Source port number specification**

```bash
nmap --source-port 53 [target]
```

A common error that many administrators are doing when configuring firewalls is to set up a rule to allow all incoming traffic that comes from a specific port number.The <code>--source-port</code> option of Nmap can be used to exploit this misconfiguration.Common ports that you can use for this type of scan are: 20, 53 and 67.

**Append Random Data**

```bash
nmap --data-length 25 [target]
```

Many firewalls are inspecting packets by looking at their size in order to identify a potential port scan.This is because many scanners are sending packets that have specific size.In order to avoid that kind of detection you can use the command <code>--data-length</code> to add additional data and to send packets with different size than the default.

**TCP ACK Scan**

```bash
nmap -sA [target]
```

It is always good to send the ACK packets rather than the SYN packets because if there is any active firewall working on the remote computer then because of the ACK packets the firewall cannot create the log, since firewalls treat ACK packet as the response of the SYN packet.

Useful resources:

- [Nmap - Techniques for Avoiding Firewalls](https://pentestlab.blog/2012/04/02/nmap-techniques-for-avoiding-firewalls/)

</details>

###### Devops Questions (5)

<details>
<summary><b>Explain how Flap Detection works in Nagios?</b></summary><br>

**Flapping** occurs when a service or host changes state too frequently, this causes lot of problem and recovery notifications.

Once you have defined **Flapping**, explain how Nagios detects **Flapping**. Whenever Nagios checks the status of a host or service, it will check to see if it has started or stopped flapping.

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

<details>
<summary><b>Is the way of distributing Docker apps (e.g. Apache, MySQL) from Docker Hub is good for production environments? Describe security problems and possible solutions. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Some of the common use cases of LXC and LXD come from the following requirements... Explain.</b></summary><br>

- the need for an isolated development environment without polluting your host machine
- isolation within production servers and the possibility to run more than one service in its own container
- a need to test things with more than one version of the same software or different operating system environments
- experimenting with different and new releases of GNU/Linux distributions without having to install them on a physical host machine
- trying out a software or development stack that may or may not be used after some playing around
- installing many types of software in your primary development machine or production server and maintaining them on a longer run
- doing a dry run of any installation or maintenance task before actually executing it on production machines
- better utilization and provisioning of server resources with multiple services running for different users or clients
- high-density virtual private server (VPS) hosting, where isolation without the cost of full virtualization is needed
- easy access to host hardware from a container, compared to complicated access methods from virtual machines
- multiple build environments with different customizations in place

</details>

<details>
<summary><b>You have to prepare a Redis cluster. How will you ensure security?</b></summary><br>

- protect a given Redis instance from outside accesses via firewall
- binding it to 127.0.0.1 if only local clients are accessing it
- sandboxed environment
- enabling **AUTH**
- enabling **Protected Mode**
- data encryption support (e.g. `spiped`)
- disabling of specific commands
- users **ACLs**

Useful resources:

- [Redis Security](https://redis.io/topics/security)
- [A few things about Redis security](http://antirez.com/news/96)

</details>

###### Cyber Security Questions (5)

<details>
<summary><b>What is OWASP Application Security Verification Standard? Explain in a few points. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is CSRF?</b></summary><br>

**Cross Site Request Forgery** is a web application vulnerability in which the server does not check whether the request came from a trusted client or not. The request is just processed directly. It can be further followed by the ways to detect this, examples and countermeasures.

</details>

<details>
<summary><b>What is the difference between policies, processes and guidelines?</b></summary><br>

As **security policy** defines the security objectives and the security framework of an organisation. A **process** is a detailed step by step how to document that specifies the exact action which will be necessary to implement important security mechanism. **Guidelines** are recommendations which can be customized and used in the creation of procedures.

</details>

<details>
<summary><b>What is a false positive and false negative in case of IDS?</b></summary><br>

When the device generated an alert for an intrusion which has actually not happened: this is **false positive** and if the device has not generated any alert and the intrusion has actually happened, this is the case of a **false negative**.

</details>

<details>
<summary><b>10 quick points on web server hardening.</b></summary><br>

Example:

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

## <a name="secret-knowledge">Secret Knowledge</a>

### :diamond_shape_with_a_dot_inside: <a name="guru-sysadmin">Guru Sysadmin</a>

<details>
<summary><b>An application encounters some performance issues. You should to find the code we have to optimize. How to profile app in Linux environment?</b></summary><br>

> Ideally, I need an app that will attach to a process and log periodic snapshots of: memory usage number of threads CPU usage.

1. You can use `top`in batch mode. It runs in the batch mode either until it is killed or until N iterations is done:

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

**This is an example of profiling a test program**

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

Also the simple way to do app profile is to use the `pstack` utility or `lsstack`.

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

I recommend in next window to click on **Self** column header, otherwise it shows that `main()` is most time consuming task.

Useful resources:

- [Tracing processes for fun and profit](http://techblog.rosedu.org/tracing-processes-for-fun-and-profit.html)

</details>

<details>
<summary><b>Using a Linux system with a limited number of packages installed, and telnet is not available. Use sysfs virtual filesystem to test connection on all interfaces (without loopback).</b></summary><br>

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
<summary><b>You should rewrite POST with payload to external API but POST requests loose the parameters passed on the URL. How to fix this problem (e.g. in Nginx) and what are the reasons for this behavior?</b></summary><br>

The issue is that external redirects will never resend **POST** data. This is written into the HTTP spec (check the `3xx` section). Any client that does do this is violating the spec.

**POST** data is passed in the body of the request, which gets dropped if you do a standard redirect.

Look at this:

```
   +-------------------------------------------+-----------+-----------+
   |                                           | Permanent | Temporary |
   +-------------------------------------------+-----------+-----------+
   | Allows changing the request method from   | 301       | 302       |
   | POST to GET                               |           |           |
   | Does not allow changing the request       | 308       | 307       |
   | method from POST to GET                   |           |           |
   +-------------------------------------------+-----------+-----------+
```

You can try with the HTTP status code **307**, a RFC compliant browser should repeat the post request. You just need to write a Nginx rewrite rule with HTTP status code **307** or **308**:

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

HTTP Status code **307** or **308** should be used instead of **301** because it changes the request method from **POST** to **GET**.

Useful resources:

- [Redirection on Apache (Maintain POST params)](https://stackoverflow.com/questions/17295085/redirection-on-apache-maintain-post-params)
- [Why doesn't HTTP have POST redirect?](https://softwareengineering.stackexchange.com/questions/99894/why-doesnt-http-have-post-redirect)

</details>

<details>
<summary><b>Write two golden rules for reducing the impact of hacked system.</b></summary><br>

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
<summary><b>How do I measure request and response times at once using <code>curl</code>?</b></summary><br>

`curl` supports formatted output for the details of the request (see the `curl` manpage for details, under `-w| -write-out 'format'`). For our purposes we’ll focus just on the timing details that are provided.

1. Create a new file, `curl-format.txt`, and paste in:

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

- `-w "@curl-format.txt"` - tells cURL to use our format file
- `-o /dev/null` - redirects the output of the request to /dev/null
- `-s` - tells cURL not to show a progress meter
`http://example.com/` is the URL we are requesting. Use quotes particularly if your URL has "&" query string parameters

</details>

<details>
<summary><b>You need to move ext4 journal on another disk/partition. What are the reasons for this? ***</b></summary><br>

To be completed.

Useful resources:

- [ext4: using external journal to optimize performance](https://raid6.com.au/posts/fs_ext4_external_journal/)
- [How to move an ext4 journal](https://unix.stackexchange.com/questions/278998/how-to-move-an-ext4-journal)

</details>

<details>
<summary><b>You're on a security conference. Members debating about putting up the OpenBSD firewall on the core of the network. Go to the podium and express your opinion about this solution. What are the pros/cons and why? ***</b></summary><br>

To be completed.

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

More slightly configuration:

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
        # Catch all in case there's a request method we're not dealing with properly
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

With fork bombs your best method for this is preventing from being to big of an issue in the first place.

</details>

<details>
<summary><b>How to recover deleted file held open by Apache?</b></summary><br>

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
<summary><b>The team of admins needs your support. You must remotely reinstall the system on one of the main servers. There is no access to the management console (e.g. iDRAC). How to install Linux on disk, from and where other Linux exist and running?</b></summary><br>

It is possible that the question should be: "_System installation from the level and in place of already other system working_".

On the example of the Debian GNU/Linux distribution.

1. Creating a working directory and downloading the system using the debootstrap tool.

```bash
_working_directory="/mnt/system"
mkdir $_working_directory
debootstrap --verbose --arch amd64 {wheezy|jessie} . http://ftp.en.debian.org/debian
```

2. Mounting sub-systems: `proc`, `sys`, `dev` and `dev/pts`.

```bash
for i in proc sys dev dev/pts ; do mount -o bind $i $_working_directory/$i ; done
```

3. Copy system backup for restore.

```bash
cp system_backup_22012015.tgz $_working_directory/mnt
```

However, it is better not to waste space and do it in a different way (assuming that the copy is in `/mnt/backup`):

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

6. In the "new" system, the next thing to do is mount the disk on which the "old" system is located (e.g. `/dev/sda1`).

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

9. And mount `proc`, `sys`, `dev` and `dev/pts` in a new working directory.

```bash
for i in proc sys dev dev/pts ; do mount -o bind $i $_working_directory/$i ; done
```

10. Install and update grub configuration.

```bash
chroot $_working_directory /bin/bash -c "grub-install --no-floppy --root-directory=/ /dev/sda"
chroot $_working_directory /bin/bash -c "update-grub"
```

11. Unmount `proc`, `sys`, `dev` and `dev/pts` filesystems.

```bash
cd
grep $_working_directory /proc/mounts | cut -f2 -d " " | sort -r | xargs umount -n
```

None of the available commands, i.e. `halt`, `shutdown` or `reboot`, will work. You need to reload the system configuration - to do this, use the **kernel debugger** (without the '**b**' option):

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
<summary><b>Rsync triggered Linux OOM killer on a single 50 GB file. How does the OOM killer decide which process to kill first? How to control this?</b></summary><br>

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

</details>

<details>
<summary><b>What are salted hashes? Generate the password with salt for the <code>/etc/shadow</code> file.</b></summary><br>

**Salt** at its most fundamental level is random data. When a properly protected password system receives a new password, it will create a hashed value for that password, create a new random salt value, and then store that combined value in its database. This helps defend against dictionary attacks and known hash attacks.

For example, if a user uses the same password on two different systems, if they used the same hashing algorithm, they could end up with the same hash value. However, if even one of the systems uses salt with its hashes, the values will be different.

The encrypted passwords in `/etc/shadow` file are stored in the following format:

```bash
$ID$SALT$ENCRYPTED
```

The `$ID` indicates the type of encryption, the `$SALT` is a random (up to 16 characters) string and `$ENCRYPTED` is a password’s hash.

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

Use the below commands from the Linux shell to generate hashed password for `/etc/shadow` with the random salt:

- Generate **MD5** password hash

```bash
python -c "import random,string,crypt; randomsalt = ''.join(random.sample(string.ascii_letters,8)); print crypt.crypt('MySecretPassword', '\$1\$%s\$' % randomsalt)"
```

- Generate **SHA-256** password hash

```bash
python -c "import random,string,crypt; randomsalt = ''.join(random.sample(string.ascii_letters,8)); print crypt.crypt('MySecretPassword', '\$5\$%s\$' % randomsalt)"
```

- Generate **SHA-512** password hash

```bash
python -c "import random,string,crypt; randomsalt = ''.join(random.sample(string.ascii_letters,8)); print crypt.crypt('MySecretPassword', '\$6\$%s\$' % randomsalt)"
```

</details>

<details>
<summary><b>You have a lot of sockets, hanging in <code>TIME_WAIT</code>. Your http service behind proxy serve a lot of small http requests. How to check and reduce <code>TIME_WAIT</code> sockets? ***</b></summary><br>

To be completed.

Useful resources:

- [How to reduce number of sockets in TIME_WAIT?](https://serverfault.com/questions/212093/how-to-reduce-number-of-sockets-in-time-wait)

</details>
