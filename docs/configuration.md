---
layout: default
title: Navigating the File System
nav_order: 2
has_children: false
permalink: /docs/navigating
---

{: .fs-6 .fw-300 }

# Writing a Basic Function
{: .no_toc }

---

Python is capable of programming many tasks, but before we can create our own projects we need to learn the basics. This section of the guide will walk you through how to create a basic palindrome function and run the file in the command line. We want to help you develop good programming habits, so we will guide you through how to write comments, docstrings and doctests to ensure your code is able to detect a palindrome word.

---

### Table of contents
{: .no_toc .text-delta }
* TOC
{:toc}

---

## What are Commands

Commands are instructions the operating system uses to perform specific tasks. Instructions provide a _layer of abstraction_ and make using a computer easy without the need to know how things work.

You can think of commands as _keywords_ _mapped_ to a mini-program that executes when you input _keywords_ into a _terminal_.

Linux commands have set syntax which allows you to pass extra _options_ and _arguments_. The syntax looks something like this:

>> _command_ [_options_] [_arguments_]

Things you should pay attention to:

* Separate commands, options, and arguments with spaces
* Short command options start with `-`
* Long command options start with `--`
* The command reads from left to right so _options_ and _arguments_ refer to the command on the left
* The type of _options_ available and _arguments_ accepted will depend on the command

![Note icon](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/icons/note.png?raw=true "Note"){: style="float: left" }
> **Note:** You can find the full information about a command by using the `man` command. The syntax is `man [command]`.

---

## Command Table

Below is a list of some commands that will be needed to follow along with this document.

**Note**: We will be using the terminal built into the PyCharm IDE.

| Command         | Description                                                                                             |
| :--------       | :------------------------------------------------------------------------------------------------------ |
| `clear`         | "Clear" your terminal screen.                                                                           |
| **[Enter]**     | Processes the command that has been typed                                                               |

---

## Writing a Palindrome Function

One of the most common introduction problems that developers solve is determining if a string is a palindrome or not. A palindrome is a word, phrase, or sequence that reads the same backward as forward.

---

**1.** Open the Pycharm application by clicking the icon from the launchpad.

![img1](https://user-images.githubusercontent.com/90500768/161899986-b0b0c2b5-2736-41b2-9986-287a625c7551.png?raw=true "PyCharm")
<!-- >![Terminal open](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/navigation/directories/term.png?raw=true "terminal") -->
<br />
<br />

**2.** Input the following command into your terminal to display your current directory.

>```
>pwd
>```

>You should be able to see exactly which directory you are currently in.

>![Screen shot pwd](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/navigation/directories/pwd.png?raw=true "pwd")
<br />
<br />

**3.** Display the contents inside your current directory with the following command.

>![Note icon](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/icons/note.png?raw=true "Note"){: style="float: left" }
>> **Note**: Using the `ls` command with the `-a` switch lists all hidden files as well.

<br />
>```
>ls
>```

>You can see a list of everything inside your current directory.

>![Screen shot ls](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/navigation/directories/contents.png?raw=true "ls")
<br />
<br />

**4.** Create a new folder inside your current directory by using the following command.

>```
>mkdir testfolder
>```

>Check the contents of your current directory again by inputting the `ls` command again.

>```
>ls
>```

>You will see that you have successfully created a new folder called *`testfolder`*.

>![Screen shot ls with testfolder](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/navigation/directories/contents2.png?raw=true "ls")
<br />
<br />

**5.** Change into the *`testfolder`* directory with the following command.

>![Note icon](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/icons/note.png?raw=true "Note"){: style="float: left" }
>>**Note**: The input after `cd` is the name of the directory you want to change into.

<br />
>```
>cd testfolder
>```

>Check to see which directory you are now currently in with the `pwd` command.

>```
>pwd
>```

>You will see that you are now inside the *`testfolder`* directory.

>![pwd2](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/navigation/directories/pwd2.png?raw=true "ls")
<br />
<br />

**6.** Change back to the previous directory with the following command.

>![Note icon](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/icons/note.png?raw=true "Note"){: style="float: left" }
>> **Note**: By adding `..`, you can jump back up one parent directory. Using `cd -` can also return you to your previous location, but you can only backtrack once.
<br />
<br />

>```
>cd ..
>```

>You can see you have returned back to the previous directory that you were in.

>![Screen shot pwd](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/navigation/directories/pwd.png?raw=true "pwd")
<br />
<br />

You now know how to open the terminal and input commands which allow you to navigate through your system. 

Now you are able to see files in your directories as well as your current directory, allowing you to easily navigate through your system.

The next step is to learn how to [create users and assign privileges.](https://dl90.github.io/linux-basics/docs/users)
