---
layout: default
---

## Introduction

The aim of this course was to furnish linguists with the basic command-line tools necessary to branch into the computational aspects of their field. Coursework included basic UNIX navigation, installing and running programs from the command line, regular expressions, basic corpus processing, basic bash scripting, version control, remote servers, and troubleshooting when (inevitably) something goes awry. Though all material was posted online, there was an optional in-person session each week during which students could receive guidance from instructors. Coursework consisted of weekly quizzes to check comprehension of the material. The class culminated in a final project, which entailed building the website you're currently viewing and hosting it on GitHub Pages.

## Week 1: The Command Line Environment

During the first week of class, we focused on the fundamentals of navigating a UNIX (or UNIX-like) environment. This included traversing filesystems with `cd` and displaying their contents with `ls`. The concept of using "flags" to increase the power and versatility of commands was also introduced. We also touched on the utility of `>` to redirect output into a less ephemeral form, such as a text file. An example of this can be seen below.

```zsh
echo Hello, World > hello.txt
```
1: basic UNIX command that causes the shell to echo a string and redirect the output into a text file

Below is a non-exhaustive list of the commands introduced in this section, along with notes on their usage and important flags where applicable.

|Command|Function|Notes/Useful Flags|
|---|---|---|
|`pwd`|Prints working directory|Useful for locating oneself in the filesystem|
|`whoami`|Prints username|Ensure one is logged in under the correct account|
|`cd`|Changes directory|Takes a directory as an argument; can be either a relative or absolute path|
|`ls`|Lists directory contents|`-a` includes hidden files; `-l` displays permissions and other helpful info|
|`cat`|Writes the contents of a file (or files) to the shell output|`-n` displays output with line numbers; can be combined with the redirect `>` command to write contents of one file to another|
|`mkdir`|Creates a new directory||
|`cp`|Copies contents of one file to another|Takes the file to copy as the first argument and the destination file as the second; the destination file will be created if it does not already exist|
|`echo`|Writes to output|Often used when writing to text files directly from the terminal|
|`touch`|Updates the timestamp of a file or creates it if it doesn't exist|Commonly used to create new files|
|`rm`|Removes a file|Does not remove directories by default, but the `-r` flag causes it to recursively delete all contents of directory; deleted material is irrecoverable and so this command should be used with caution|
|`rmdir`|Removes a directory|Only works on empty directories and thus is far safer than `rm -r`|


## Week 2: Navigating a UNIX System

In the second week of class, we furthered our exploration of the UNIX environment by learning about file permissions, process management, and remote server access. First, we touched on the various types of permissions available for a given file and how to modify them with the `chmod` command. These permissions consist of:

* Read- Governs whether a user can view the contents of a file
* Write- Governs whether a user can modify the file
* Execute- Governs whether a user can run the file

These permissions in turn can be distributed freely across the following identities:

* Owner (u)- The file's creator
* Group (g)- Users in the same group as Owner
* Other (o)- Users not in Owner's group

The `chmod` command can distribute permissions using either symbolic or octal notation. Both of the following commands have the effect of giving Owner read and write permissions to a file while making it read-only to all others.

Symbolic:
```zsh
chmod u+rw,go+r file_name
```
Octal:
```zsh
chmod 644 file_name
```

Next, we learned about managing processes from the command line. In particular, the `ps` command with optional `-f` flag were discussed. This is used to display all processes currently running, which can be subsequently killed using the `kill` command.

Finally, we set up credentials with the University of Helsinki's Puhti server in order to practice remote server access. We used the `ssh` command to log in to the server and `scp` to move files between the server and our local machine. 

## Week 3: Basic Corpus Processing

```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```

## Week 4: Advanced Corpus Processing

```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```

## Week 5: Scripting and Configuration Files

```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```

## Week 6: Installing Programs

```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```

## Week 7: Version Control

```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```

## Final Project

```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```