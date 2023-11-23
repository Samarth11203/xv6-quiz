# XV Quiz (CSL 3030)

Welcome to the XV Quiz for CSL 3030 - Operating Systems!



## Instructions
- Answer the multiple-choice questions by selecting the correct option.
- For theoretical questions, provide concise and accurate explanations.
- Feel free to use this quiz for self-assessment or educational purposes.

## Multiple-Choice Questions

#### Question 1: Basics
1. What is XV6?
   - a. A programming language
   - b. A Unix-like operating system
   - c. A file system
   - d. An assembly language

#### Question 2: Architecture
2. XV6 is based on which earlier operating system?
   - a. Windows
   - b. Linux
   - c. BSD
   - d. DOS

#### Question 3: File System
3. Which file system is used in XV6?
   - a. FAT32
   - b. NTFS
   - c. ext4
   - d. simple

#### Question 4: System Calls
4. How are system calls implemented in XV6?
   - a. As functions in the C standard library
   - b. As interrupts
   - c. Through the command line
   - d. As external programs

#### Question 5: Processes
5. In XV6, what is the maximum number of processes that can run simultaneously?
   - a. 128
   - b. 256
   - c. 512
   - d. 1024

#### Question 6: Shell
6. What is the name of the shell used in XV6?
   - a. Bash
   - b. Zsh
   - c. Sh
   - d. Fish

#### Question 7: Scheduling
7. How does XV6 handle process scheduling?
   - a. Round-robin scheduling
   - b. Priority-based scheduling
   - c. First-Come-First-Serve (FCFS)
   - d. Random scheduling

#### Question 8: Memory Management
8. Which memory management technique is used in XV6?
   - a. Paging
   - b. Segmentation
   - c. Virtual Memory
   - d. None of the above

#### Question 9: Interrupts
9. How are interrupts handled in XV6?
   - a. Through polling
   - b. Using hardware interrupts
   - c. Using software interrupts
   - d. Both b and c

#### Question 10: Multithreading
10. Does XV6 support multithreading?
    - a. Yes
    - b. No

#### Bonus Question:
11. Who developed XV6?
    - a. Microsoft
    - b. Google
    - c. MIT
    - d. IBM

## Theoretical Questions

#### Question 12: Process States
12. Briefly explain the different states a process can be in within the XV6 operating system.

#### Question 13: File System Structure
13. Describe the structure of the file system in XV6. Include the key components and their roles.

#### Question 14: System Calls vs. Library Functions
14. Explain the difference between system calls and library functions in the context of XV6. Provide examples of each.

#### Question 15: Memory Paging
15. How does memory paging work in XV6? Discuss the benefits of using paging in memory management.

#### Question 16: Shell Commands
16. Name and briefly explain three essential shell commands in the XV6 operating system.

#### Question 17: Process Synchronization
17. Discuss the concept of process synchronization in XV6. Why is it essential, and what mechanisms are used to achieve it?

#### Question 18: Interrupt Handling
18. Explain the role of interrupts in the XV6 operating system. How are interrupts handled, and what is their significance in system operation?

#### Question 19: Virtual Memory
19. What is virtual memory, and how is it implemented in XV6? Discuss the advantages of using virtual memory.

#### Question 20: Boot Process
20. Outline the steps involved in the boot process of XV6. What happens from the moment the computer is powered on to when the XV6 kernel is loaded into memory?

## Answers
Please write your answers here
1. b. A Unix-like operating system
2. c. BSD
3. d. simple
4. b. As interrupts
5. a. 128
6. c. Sh
7. a. Round-robin scheduling
8. a. Paging
9. d. Both b and c
10. b. No
11. c. MIT
12. There are 6 states of process in xv6 namely a) Unused b) Embryonic c) Sleeping d) Runnable e) Running f) Zombie
Unused : Process is not allocated currently.
Embryonic : Process is created but not in use.
Sleeping : Process is in waiting state and will be executed if the signal is available for execution.
Runnable : Process is ready to run and when the schedular will schedule it, it will be executed.
Running : Process is currenctly running by the cpu.
Zombie : Process is executed but its exit code is not collected by the parent.
13. File System Structure in XV6 comprises of a) Inodes, b) Data Blocks, c) Superblock, d) Directory Entries
Inodes: It contains the metadata about the directories, files, etc.
Data Blocks: It contains the content of the file which are there in inodes.
Superblock: It contains the overall metadata/data of the file system in xv6.
Directory Entries: It contains the filename of the directories present in inodes.
14. Difference between System Calls and Library Functions in XV6
System Calls: It interacts with the kernel throught the kernel interface. For example : fork(), read(), etc.
Library Functions: It contains functions which are called by user or directly by the applications at user-level. For example : printf(), scanf(), etc.
15. Memory Paging is used to create the map or association between the virtual and physical memory spaces using the pages format.
Benefits : It simplifies the memory management and also the virtual memory space allocation. It can be used to perform the demand paging also.
16. Shell commands available in xv6 are : ls, cd, sh
ls: Lists files and directories in the current location.
cd: We can change the directory using this command.
sh: It is used to run the script files.
17. Process Synchronization in XV6 ensures the execution of process in such a way that it will not create the deadlocks or access the shared memory as intended. It also manages the shared resource.
Mechanisms in XV6:
Locks and Semaphores: Used to control access to shared resources.
18. Interrupt Handling in XV6
The execution flow of the process is disturbed when interrution occurs.
Hardware and software events are used to handle it in xv6, allowing the system to manage the processes systematically by keeping track of some outer signals.
19. Virtual Memory in XV6
Virtual memory is an abstraction that provides each process with its own address space. It creates the illusion of more extensive memory than physically available.
Implementation in XV6:
Paging: Maps virtual to physical addresses.
Page Faults: Triggered when a required page is not in physical memory.
Advantages:
Each process has its own address space.
Non-contiguous allocation simplifies memory management.
Efficient use of physical memory.
20. Boot Process in XV6
Power-On: Computer is powered on.
BIOS/UEFI: Executes, performs POST, and locates bootable device.
Bootloader: Loaded and executed.
Kernel Loading: Bootloader loads the xv6 kernel into memory.

