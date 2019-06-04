# Operating-System-Poster-Presentation
![os1-min](https://user-images.githubusercontent.com/33459977/56201988-afda7500-605f-11e9-8393-86b6830b1a07.png)

[PSD File](https://drive.google.com/open?id=1b5Uu1az8cXtIedeBFr-d27iyVXJa3Uia)

## Process Management
Do you think your Linux computer will automatically take care of everything by itself? Sometimes you may need to step in directly.
Process management is a case in point. Linux creates a process whenever a program is launched, either by you or by Linux. This process is a container of information about how that program is running and what’s happening.

There are fundamentally two types of processes in Linux:

Foreground processes (also referred to as interactive processes) – these are initialized and controlled through a terminal session. In other words, there has to be a user connected to the system to start such processes; they haven’t started automatically as part of the system functions/services.
Background processes (also referred to as non-interactive/automatic processes) – are processes not connected to a terminal; they don’t expect any user input.

There are two conventional ways used for creating a new process in Linux:

#### Using The System() Function 
This method is relatively simple, however, it’s inefficient and has significantly certain security risks.
#### Using fork() and exec() Function
This technique is a little advanced but offers greater flexibility, speed, together with security.

[For more reading](https://www.tecmint.com/linux-process-management/) 

![os2-min](https://www.tecmint.com/wp-content/uploads/2017/03/ProcessState.png)


## File Management

In Linux, the directories can be divided into two classifications:

Root Directory → It is denoted by ” / ” (forward slash). Root directory is the root/base of the entire file system and cannot be renamed or deleted. There can be only one root directory.
Sub Directories → Directories that are under the root ( / ) directory are called sub-directories.

#### FileSystem Hierarchy Standard (FHS)

The FileSystem Hierarchy Standard (FHS) defines the directory structure and directory contents in a Linux distribution. It also defines the names, permissions and locations for several file types and directories. All files and directories appear under one common root directory, even if they are stored on different devices physically. The root is the parent directory to all other directories

[For more reading](https://thesagediary.com/2018/09/26/linux-file-system-directory-architecture/) 

![os3-min](https://thesagediary.files.wordpress.com/2018/09/linuxfilesystem.png?w=1024)


## Memory Management

Since the early days of computing, there has been a need for more memory than there exists physically in a system. Strategies have been developed to overcome this limitation and the most successful of these is virtual memory. Virtual memory makes the system appear to have more memory than it actually has by sharing it between competing processes as they need it. This sleight of hand is invisible to those processes and to the users of the system. Virtual memory allows:

#### Large Address Spaces
The operating system makes the system appear as if it has a larger amount of memory than it actually has. The virtual memory can be many times larger than the physical memory in the system,
#### Fair Physical Memory Allocation
The memory management subsystem must fairly share the physical memory of the system between the running processes in the system,
#### Protection
Memory management ensures that every process in the system is protected from all other processes; in this way a crashing application cannot affect other processes or the operating system itself.
#### Shared Virtual Memory
Virtual memory allows two processes to share memory between themselves, for example use a shared library. Shared libraries mean that library code only needs to exist in one place and not be duplicated in every application.

[For more reading 1](http://www.admin-magazine.com/Archive/2014/21/Managing-Linux-Memory) , 
[For more reading 2](http://www.science.unitn.it/~fiorella/guidelinux/tlk/node24.html )

![os4-min](http://www.admin-magazine.com/var/ezflow_site/storage/images/archive/2014/21/memory-management-on-high-end-systems/figure-2/91088-1-eng-US/Figure-2_large.png)

## I/O Management

Management of I/O devices is a very important part of the operating system - so important and so varied that entire I/O subsystems are devoted to its operation. ( Consider the range of devices on a modern computer, from mice, keyboards, disk drives, display adapters, USB devices, network connections, audio I/O, printers, special devices for the handicapped, and many special-purpose peripherals. )
I/O Subsystems must contend with two ( conflicting? ) trends: (1) The gravitation towards standard interfaces for a wide range of devices, making it easier to add newly developed devices to existing systems, and (2) the development of entirely new types of devices, for which the existing standard interfaces are not always easy to apply.
Device drivers are modules that can be plugged into an OS to handle a particular device or category of similar devices.

[For more reading](https://www.cs.uic.edu/~jbell/CourseNotes/OperatingSystems/13_IOSystems.html)

![os5-min](https://www.cs.uic.edu/~jbell/CourseNotes/OperatingSystems/images/Chapter13/13_01_TypicalBus.jpg)
