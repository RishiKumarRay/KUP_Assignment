**Que-1 -> What is GNU Project ?**

The name of the GNU project is derived from the recursive acronym "GNU's Not Unix." Unix was a very popular operating system in the 80s, so Stallman designed GNU to be mostly compatible with Unix so that it would be convenient for people to migrate to GNU.

Stallman established the Free Software Foundation in October 1985 to assist administrative, legal, and organisational aspects of the GNU project and also to spread the use and knowledge of Free Software. The main licences of the GNU project are the GNU General Public License (GPL) and the GNU Lesser General Public License (LGPL, originally called GNU Library General Public License). Over the years they have become established as the most widely used licences for Free Software.

**Que -2 -> What is the difference between UNIX and Linux?**

|                            Linux                             |                             Unix                             |
| :----------------------------------------------------------: | :----------------------------------------------------------: |
| Linux is open source and can be freely distributed,downloaded, and distributed. | Unix was developed by AT&T Labs, different commercial vendors, and non-profit organizations. |
|                It has huge Community Support                 |           It has less community support than linux           |
|           It supports more file system than Unix.            |                It suppoets lesser than linux                 |
| Linux is used everywhere from servers, PC, smartphones, tablets to mainframes and supercomputers. |         It is used in servers, workstations and PCs.         |

**Que -3 What do you mean by Integrity check of BIOS? Mention firmwares other than BIOS ?**

The system integrity test performed by BIOS is called POST(Power On Self Test). POST include routines performed by the firmware once the device is switched on to verify if the hardware is performing as expected otherwise return error messages and beeps. The harware checked include RAM, processors, peripheral devices etc. Firmwares other than Bios are UEFI.

**Que -4 What is a UEFI?**

UEFI stands for Unified Extensible Firmware Interface. It does the same job as a BIOS, but with one basic difference: it stores all data about initialization and startup in an .efi file, instead of storing it on the firmware.

**Que -5 What is the difference between BIOS & UEFI?**

|                             BIOS                             |                             UEFI                             |
| :----------------------------------------------------------: | :----------------------------------------------------------: |
|           It stands for basic input output system.           |     It stands for Unified Extensible Firmware Interface.     |
| It is stored on an EPROM (Erasable Programmable Read-Only Memory). | It stores all data about initialization and startup in an .efi file, instead of storing it on the firmware. |
|        BIOS supports drive sizes upto 2.2 terabytes.         |         UEFI supports drive sizes upto 9 zettabytes          |
|              UEFI runs in 32bit or 64bit mode.               |                   Whereas Bios only 16 bit                   |

**Que 6 -  When should you go for Ubuntu & when for other systems?**

When you want more interaction with GUI one can go for windows or mac as it is more GUI based. one can go for ubuntu as it is open source and more fast , more privacy with high customisation and don't want to pay like in windows. 

**Que 7- List various linux distributions & their use cases ?**

Ubuntu - It came into existence in 2004 by Canonical and quickly became popular. Ubuntu is a next version of Debian and easy to use for newbies. It comes with a lots of pre-installed apps and easy to use repositories libraries.

Debian - Debian has its existence since 1993 and releases its versions much slowly then Ubuntu and it is much more stable than ubuntu.

RHEL - It is known as red hat enterprise linux and it is commercial and it always provides support since it is paid.

Centos:- CentOS is a community project that uses red hat enterprise Linux code but removes all its trademark and make it freely available. In other words, it is a free version of RHEL and provide a stable platform for a long time.

Fedora - It is a project that mainly focuses on free software and provides latest version of software. this project is supported by red hat.

**Que 8- What does a systemd.unit(5) means?**

It represents the 5th section of man page of systemd.unit

**Que 9- What are getty commands and uname command?**

Uname Command is used for displaying the information about this system. SYNTAX- uname [option] OPTIONS-

1. -a: It prints all the system information in the following order: Kernel name, network node hostname, kernel release date, kernel version, machine hardware name, hardware platform, operating system Syntax: $uname -a
2. -s: It prints the kernel name. Syntax: $uname -s
3. -n: It prints the hostname of the network node (current computer). Syntax: $uname -n
4. -r: It prints the kernel release date. Syntax: $uname -r
5. -v: It prints the version of the current kernel. Syntax: $uname -v
6. -m: It prints the machine hardware name. Syntax: $uname -m
7. -p: It prints the type of the processor. Syntax: $uname -p
8. -i: It prints the platform of the hardware. Syntax: $uname -i
9. -o: It prints the name of the operating system. Syntax: $uname -o

getty, short for "get tty", is a Unix program running on a host computer that manages physical or virtual terminals (TTYs). When it detects a connection, it prompts for a username and runs the 'login' program to authenticate the user.

**Que 10- What is squashfs file system?**

This is used when creating tiny-sized and embedded Linux systems, every byte of the storage device (floppy, flash disk, etc.) is very important, so compression is used everywhere possible. For huge public archives, as well as for personal media archives, this is essential. It is a read-only file system that lets you compress whole file systems or single directories, write them to other devices/partitions or to ordinary files, and then mount them directly (if a device) or using a loopback device (if it is a file).

**Que 11- What are /dev/loop and /dev/tty ?**

/dev/tty stands for the controlling terminal (if any) for the current process (the process that uses "/dev/tty" in a command). To find out which tty's are attached to which processes use the "ps -a" command at the shell prompt (command line).

**Que 12- What are Linux Signals?**

A signal is a notification to a process that an event has occurred. Signals are sometimes described as software interrupts, because in most cases, they interrupt the normal flow of execution of a program and their arrival is unpredictable.

**Que 13 - What is the purpose of creating and using hidden files.**

The purpose of the hidden files are to prevent it from getting deleted accidently that doesn't mean we cannot delete that.

**Que 14- How ext4fs is faster/better?**

It is faster because it supports delayed allocation that means a file which is written , the appended part is stored in the memory like cache and RAM and after a time it is written in harddisk and it is also called as writeback time.

**Que 15- What is swap & swap memory?**

Swap is hard disk space used as RAM. It is (relatively speaking) very slow, but stops computers from crashing when they are trying to deal with more data then their RAM can handle.

Swap space is a space on a hard disk that is a substitute for physical memory. It is also called a swap file. This interchange of data between virtual memory and real memory is called swapping and space on disk as “swap space”.

swap memory is the dedicated amount of hard drive that is used whenever RAM runs out of memory**.**

**Que 16- How to mount a file system?**

To mount a file system we can make use of this command :

mount -t Type Device MountPoint

here mount point can be created by mkdir

**Que 17- Mention a ZFS use case.**

It has pooled storage i.e ZFS combines the features of a file system and a volume manager. This means that unlike other file systems, ZFS can create a file system that spans across a series of drives or a pool. Not only that but you can add storage to a pool by adding another drive.

It has also copy on write i.e On ZFS, the new information is written to a different block. Once the write is complete, the file systems metadata is updated to point to the new info. This ensures that if the system crashes (or something else happens) while the write is taking place, the old data will be preserved while in other system it lost forever.

It also has data integrity verfication which means Whenever new data is written to ZFS, it creates a checksum for that data. When that data is read, the checksum is verified. If the checksum does not match, then ZFS knows that an error has been detected. ZFS will then automatically attempt to correct the error.

The main reason why people advise ZFS is the fact that ZFS offers better protection against data corruption as compared to other file systems. It has extra defences build-in that protect your data in a manner that other free file systems cannot and it provies facility to increase storage**.**

**Que 18- How to check the port number of a process?**

We can use netstat or ss command also

**Que 19- What is unix time sharing (UTS)?**

A UNIX Time‑Sharing (UTS)  is a namespace that allows a single system to appear to have different host and domain names to different processes.

**Que 20-  What are control groups?**

Cgroups or Control groups is a Linux kernel feature that limits the resource usuage such CPU or RAM. 

**Que 21- What is the difference between sbin & usr/sbin?**

Sbin contains the binaries that are run by a sudo user or super user but in the case of usr/sbin it is spefic to the user that we have on our system.

**Que 22- Examples of awk, grep and sed**

***Grep*** command is used for finding particular patterns in a file and to display all the fields matching that pattern.

Suppose we want to find a word manager common in a file then we can do this by

grep -i "manager" example.txt (here i is used as to ignore case senstivity)

likewise we can use this grep command with different options

**Awk** command is more of scripting language used in manipulating data and generating reports.

When using ‘awk’ we enclose patterns in curly braces. Both pattern and action form a rule and the entire awk program is enclosed in single quotes.

awk '{print}' example.txt (here since pattern is not specified it will print all)

awk '/manager/ {print}' example.txt

it wil print containing managers.

awk ‘NR==3, NR==6 {print NR,$0}’ example.txt

It will display from line number 3 to number 6.

**SED** is short for stream editor. It can be used to perform different functions such as searching.

sed 's/manager/operations/g' test

To replace only on a specific line, specify the file line as below where we are replacing on the third line.

sed '3 's/manager/operations/g' test

here we wil also use i flag to save the file

sed -i 's/manager/operations/g' test

**Que 23- How many tables are there in iptables?**

There are Basically 5 tables in iptables-

- Input table
- NAT table
- Mangle table
- Raw table
- Security

**Que 24: What are prot, opt , Source , and Destinations ?**

prot:-This defines the protocol (TCP,IP) of the packet.

source:- This tells the source address of the packet.

destination:- This defines the destination address of the packet

opt :- Special options for that specific rule

**Que 25- Why rules are added to the top?**

The Rules we set in the iptables are checked from the topmost rules to the bottom. Whenever a packet passes any of the top rules, it is allowed to pass the firewall. The lower rules are not checked, So that's why rules are added to the top.

**Que 26- What type of rules we can add to the iptables?**

There are basically 3 rules or policies that we can add in the iptables:

- ACCEPT
- DROP
- REJECT

ACCEPT - when the traffic passes the rules in its specified chain then iptables accept the traffic and it opens it gates and allows it to pass.

DROP - when the traffic is unable to pass the rules then the iptable blocks the traffic.

Reject - here this is similar to Reject but in this case a message is sent to the sender which states that the transfer is not reachable or its failed.

**Que 27: Can we block a website by its domain name only ?**

Yes we can do this and we can block the website by its domain name with using this command :

iptable -I INPUT -s [www.facebook.com](http://www.facebook.com/) -j DROP

**Que 28: How can we persist rules in an iptable?**

Inorder to do this first we have to download persistant package then we can run this command

These can be saved in a file with the command `iptables-save` for IPv4.

sudo iptables-save > /etc/iptables/rules.v4

**Que 29: How can we save rules in an iptable?**

through persisting we can save rules in ipv4 or ipv6.

**Que 30- What is the difference between ufw & iptables.**

| UFW                                                          | IPtable                                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| UFW is a simplified firewall mechanism that is implemented on top of iptables. | Iptables is a kernel level ip filtering mechanism. It does allow you to make routing decisions and so on on IP packets. |
| UFW is not as flexible but is easier to configure for common scenarios. | To use IPtables you need to understand TCP/IP connections, more complicated protocols |

**Que 31-  What are public & private keys?**

An SSH key relies upon the use of two related keys, a public key and a private key, that together create a key pair that is used as the secure access credential. The private key is secret, known only to the user, and should be encrypted and stored safely. The public key can be shared freely with any SSH server to which the user wishes to connect.

**Que 32- How SSH works ?**

The SSH protocol is based on the client-server model. Therefore, an SSH client must initiate an SSH session with an SSH server. Most of the connection setup is conducted by the SSH client and public key is used to verify the identity of the SSH server, and then symmetric key encryption and hashing algorithms are used.

**Que 33 - What is the difference between HTTP and HTTPs?**

HTTPS is HTTP with encryption. The difference between the two protocols is that HTTPS uses TLS (SSL) to encrypt normal HTTP requests and responses. As a result, HTTPS is far more secure than HTTP.

**Que 34 - What is SSL?**

*SSL* (*Secure Sockets Layer*) is a protocol for establishing secure links between networked computers.

**Que 35 - What is the difference between apt update and apt-upgrade ?**

“apt-get update” updates the package sources list to get the latest list of available packages in the repositories and “apt-get upgrade” updates all the packages presently installed in our Linux system to their latest versions.

**Que 36 - What do repositories contain in a linux system?**

A Linux repository is a storage location from where your system retrieves and installs updates and applications also each repository is a collection of the software that are hosted on a remote server and intended to be used for installing and updating software packages on Linux systems.

**Que 37 - What are the package managers used in Linux?**

Package managers are the tools that work to install, update, upgrade packages in linux.

**Que 38 -What does the number represent after the file permissions?**

Those numbers represnt the total number of directories present 

**Que 39 -What is the difference between apt and apt-get?**

The basic difference between apt and apt-get is apt shows the number of packages that can be upgraded while it is not in the case of the apt-get also in the case of apt there is a improve design and additional details.

**Que 40- How can I give access to someone to my AWS instance?**

We can give access to someone by copying their public key in our authorized keys directory.

**Que 41- What are daemon applications?**

Daemon applications are the ones which runs in background.

**Que 42- What does a ".d" represent after a filename?**

Here d stands for directory and contains the configuration files

**Que 43-  What happens when a pem file gets deleted?**

If this happens then we will not be able to access our instance

**Que 44- What information is stored in the /etc/host file?**

This files stores about the hostname

**Que 45- What is SCP & what does this command do?**

This command is used for securely copying files between local host and remote or between 2 remote host.

```
scp /path/file_name ubuntu@ip destination
here file name is the file we wish to transfer
```

**Que 46-  How port forwarding works?**

 Port forwarding is a technique that is used to allow external devices access to computers services on private networks. Local port forwarding is the most common type of port forwarding. It is used to let a user connect from the local computer to another server.

**Que 47- How can we connect without IP to AWS instance?**

we can define the ip addresses in hostname in sshd config file and through that we can make a connection.

**Que 48- What is an ssh agent?**

ssh agent is like a key manager and it contains the keys and certificates for connecting through a server.

here using this ssh agent to connect without typing pass phrase every time.

**Que 49-  Create a unit file for any application.**

This is the unit file that we created for nginx during sessions-

|      |[Unit]                                                       |
| ---- | ------------------------------------------------------------ |
|      | Description=A high performance web server and a reverse proxy server |
|      |                                                              |
|      | After=network.target                                         |
|      |                                                              |
|      | [Service]                                                    |
|      | Type=forking                                                 |
|      | PIDFile=/run/nginx.pid                                       |
|      | ExecStartPre=/usr/sbin/nginx -t -q -g 'daemon on; master_process on;' |
|      | ExecStart=/usr/sbin/nginx -g 'daemon on; master_process on;' |
|      | ExecReload=/usr/sbin/nginx -g 'daemon on; master_process on;' -s reload |
|      | ExecStop=-/sbin/start-stop-daemon --quiet --stop --retry QUIT/5 --pidfile /run/nginx.pid |
|      | TimeoutStopSec=5                                             |
|      | KillMode=mixed                                               |
|      |                                                              |
|      | [Install]                                                    |
|      | WantedBy=multi-user.target                                   |

**Que 50- What is RHEL?**

RHEL is red hat enterprise linux, it is based out on red hat and is commerical i.e we have to pay for it and it comes with red hat support and provides many features to users. the package managers found in red hat are YUM and RPM.



