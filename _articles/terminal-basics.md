---
layout: article
title: Learn Linux Terminal Basics
description: >
  Linux offers users a lot of flexibility. There's always more than one way to complete a task, and using the terminal is one of them.
keywords:
  - Linux
  - Ubuntu
  - Ubuntu Beginner
  - Linux Terminal
  - System76
  - Technical Support
hidden: false
section: faq

---

The <u>Terminal</u> is an interactive, text-based interface for your Ubuntu Operating System. When you type a command, you're basically telling your computer to do something very specific. Many commands will print information to the screen. Some will ask for input, and others may just return you to a prompt.

The quickest way to install, remove or update applications is through the <u>Terminal</u>. The <u>Terminal</u> is also referred to as the shell, command line, prompt, or command prompt.

To open a <u>Terminal</u>, press <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>T</kbd> or tap the <kbd><span class="fl-ubuntu"></span></kbd> to search your computer and type the word <u>Terminal</u>.

A box like the one below will appear:

![Ubuntu Terminal](/images//ubuntu-terminal/terminalmain.png)

### Navigating The Terminal

It might not look like much, and at first glance there might not appear to be much information, but the <u>Terminal</u> is one of the most powerful tools at your disposal. Take a look:

![Ubuntu Terminal Overview](/images//ubuntu-terminal/overview.png)

Section | Description
--------|------------
Current User | The username of the person currently logged in to this <u>Terminal</u>.
Current Host | The hostname of the system currently in use by the <u>Terminal</u>. Unless you've connected to a remote machine via SSH, this will be the same name as your computer.
Current Directory | The current folder that this <u>Terminal</u> resides in. Commands entered and files modified are scoped to this folder, unless providing an absolute path to another file or folder, or if the command is available in the user's $PATH. Basically, the <u>Terminal</u> can only see into this folder. A tilde (~) indicates the user's home directory, `/home/emma` for example.
Prompt | Anything entered after this symbol is interpreted as a command.
Cursor | A visual indicator of the user's current position in the <u>Terminal</u>.

As you change folders and move throughout your computer, the prompt will change in response. In many cases, you won't need to move around to run a command.

To list all files and folders in the current directory, type `ls`. To change directories (folders), type `cd [directory name]`. To go back up a directory type `cd ..`. At any time, you can press the Tab key to have the <u>Terminal</u> guess the completion for your entry, or twice to show all possibilities.

![Moving around](/images//ubuntu-terminal/moving-around.png)

### Running Elevated Commands

In most cases, the <u>Terminal</u> prevents you from damaging your system by requiring authentication or elevated privileges to run certain commands. For example, to check for updates you will need to prepend the command `apt update` with `sudo`. Below is an example of the same command, ran once without `sudo` and once with. 

![Using sudo](/images//ubuntu-terminal/sudo.png)

When you run a command with `sudo` in front of it, you'll be prompted for your password. When typing your password, you won't see anything. Just enter your password and then press <kbd>Enter</kbd>. If it's entered incorrectly, the <u>Terminal</u> will let you know and give you another chance to enter your password.

## Useful Commands:

```
sudo apt update
```

This command will tell your system to search for potential updates and advise if there are any available, but this command does not install them.

```
sudo apt upgrade
```

This command will download and apply any updates to your System76 computer.

```
sudo apt install [application]
```

This will install a particular application and its dependencies on your computer.

```
sudo apt purge [application]
```

This will remove a program and it's configuration files from your computer.

```
man sudo
```

The `man` command is short for manual. You can type the `man` command in front of any command that you want more information about.