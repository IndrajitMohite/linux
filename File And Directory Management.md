# <a name="File And Directory Management"></a>File And Directory Management
#Sudo Admin @IndrajitMohite
**Table of Contents**
* [Problem Statement](#problem-statement)
* [File System](#file-system)

* [Answere](#answere)
    * [Command Structure](#command-structure)
* [Command Help](#command-help)


<br>
## <a name="problem-statement"></a>Problem Statement
Commands and short-cuts pack much more punch than that on a terminal
      1.	Create file structure as follows using file/directory utility commands. Here F1 and S1 are files and rest are Directories

      2.	Add Contents in F1 File and S1 File.
      3.	Display Current working directory.
      4.	Go to SY Directory. Copy S1 file to TY Directory with name S2.
      5.	Being present in SY Directory Move F1 file from FY Directory to B Tech Directory.
      6.	Remove S1 File from SY Directory.
      7.	Display number of lines form S2 file.
      8.	Display number of characters form S2 file.
      9.	Compare files F1 and S2 files and explain about the output.
      10.	Use Diff command on F1 and S2 files. And explain the output observed.
      11.	Display first 7 lines from F1 file,
      12.	Display last 7 lines from F1 file,
      13.	Remove duplicate lines from the F1 file and display the output.
      14.	Sort the file contents of file F1.
      15.	Display the current month with full name.



<br>

## <a name="file-system"></a>File System

Before we dive into interesting commands, lets get a brief on Linux file system. 

* `man hier` gives description of the filesystem hierarchy. A few examples:
    * `/` This is the root directory. This is where the whole tree starts.
    * `/bin` This directory contains executable programs which are needed in single user mode and to bring the system up or repair it.
    * `/home` On machines with home directories for users, these are usually beneath this directory, directly or not. The structure of this directory depends on local administration decisions.
    * `/tmp` This directory contains temporary files which may be deleted with no notice, such as by a regular job or at system boot up.
    * `/usr` This directory is usually mounted from a separate partition. It should hold only sharable, read-only data, so that it can be mounted by various machines running Linux.
    * `/usr/bin` This is the primary directory for executable programs. Most programs executed by normal users which are not needed for booting or for repairing the system and which are not installed locally should be placed in this directory.
    * `/usr/share` This directory contains subdirectories with specific application data, that can be shared among different architectures of the same OS. Often one finds stuff here that used to live in /usr/doc or /usr/lib or /usr/man.


<br>

## <a name="answere"></a>answere

Command Line Interface (CLI) allows us interact with computer using text commands

For example: the `cd` command would help navigating to a particular directory and `ls` command to view contents of a directory. In GUI,

    
#### <a name="command-structure"></a>Command Structure

Start
```bash
indrajit@ubuntu:~$ //indrajit mohite 
 
indrajit@ubuntu:~$ ls 
Desktop    Downloads  it     Pictures  sample.txt  Templates 
Documents  indrajit   Music  Public    snap        Videos
```

Problem Statement 1 
  1.	Create file structure as follows using file/directory utility commands. Here F1 and S1 are files and rest are Directories
<br>

```bash
indrajit@ubuntu:~$ mkdir Class 
indrajit@ubuntu:~$ cd Class 
indrajit@ubuntu:~/Class$ mkdir FY 
indrajit@ubuntu:~/Class$ mkdir SY 
indrajit@ubuntu:~/Class$ mkdir TY 
indrajit@ubuntu:~/Class$ mkdir BTech 
indrajit@ubuntu:~/Class$ ls 
BTech  FY  SY  TY 
indrajit@ubuntu:~/Class$ cd FY
```

  * `mkdir` command create new directory 
	* `cd` help to open dir `help` command
	* `ls` List Directories 
  
Problem Statement 2
   2.	Add Contents in F1 File and S1 File.
```
indrajit@ubuntu:~/Class/FY$ cat > F1.txt 
This is the new File Name F1 created 
thank you.indrajit@ubuntu:~/Class/FY$ cd .. 
indrajit@ubuntu:~/Class$ cd SY 
indrajit@ubuntu:~/Class/SY$ cat > S1.c 
This is the new .C File Name S1 created 
Thank You.indrajit@ubuntu:~/Class/SY$ cd .. 
```



<br>

#### <a name="command-structure"></a>Command Structure

only the command

* `clear` clear the terminal screen
* `top` display Linux processes

command for list

* `ls -l` list directory contents, use a long listing format


command for Directory

* `mkdir project` create directory named 'project' in current working directory


command for delete

* `rm -r project` remove 'project' directory 
<br>



```bash
$ echo '$SHELL'
$SHELL

$ echo "$SHELL"
/bin/bash
```
<br>


